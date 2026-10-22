# safepeopleregistry_api_sdk.OrganisationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**organisations_appoint_sro**](OrganisationsApi.md#organisations_appoint_sro) | **PUT** /api/v1/organisations/{id}/sro | organisations@appointSro
[**organisations_invite_sro**](OrganisationsApi.md#organisations_invite_sro) | **POST** /api/v1/organisations/{id}/sro/invite | organisations@inviteSro
[**organisations_remove_delegate**](OrganisationsApi.md#organisations_remove_delegate) | **DELETE** /api/v1/organisations/{id}/delegates/{userId} | organisations@removeDelegate
[**organisations_resend_sro_invite**](OrganisationsApi.md#organisations_resend_sro_invite) | **POST** /api/v1/organisations/{id}/sro/resend_invite | organisations@resendSroInvite


# **organisations_appoint_sro**
> OrganisationsAppointSro200Response organisations_appoint_sro(id, organisations_appoint_sro_request)

organisations@appointSro

Hands the SRO role over immediately: the appointee becomes SRO, the current SRO becomes a delegate, and an invited SRO keeps their invitation but will join as a delegate. Delegates can appoint while the organisation has no claimed SRO; after that only the SRO can.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisations_appoint_sro200_response import OrganisationsAppointSro200Response
from safepeopleregistry_api_sdk.models.organisations_appoint_sro_request import OrganisationsAppointSroRequest
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.OrganisationsApi(api_client)
    id = 1 # int | organisations entry ID
    organisations_appoint_sro_request = safepeopleregistry_api_sdk.OrganisationsAppointSroRequest() # OrganisationsAppointSroRequest | 

    try:
        # organisations@appointSro
        api_response = api_instance.organisations_appoint_sro(id, organisations_appoint_sro_request)
        print("The response of OrganisationsApi->organisations_appoint_sro:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_appoint_sro: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| organisations entry ID | 
 **organisations_appoint_sro_request** | [**OrganisationsAppointSroRequest**](OrganisationsAppointSroRequest.md)|  | 

### Return type

[**OrganisationsAppointSro200Response**](OrganisationsAppointSro200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**403** | Forbidden |  -  |
**404** | The user is not a claimed member of this organisation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_invite_sro**
> OrganisationsInviteSro201Response organisations_invite_sro(id, organisations_invite_sro_request)

organisations@inviteSro

Creates an invited (unclaimed) SRO and emails them an invitation. The current SRO keeps the role until the invitee claims their account; any other invited SRO keeps their invitation but will join as a delegate. Delegates can invite while the organisation has no claimed SRO; after that only the SRO can.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisations_invite_sro201_response import OrganisationsInviteSro201Response
from safepeopleregistry_api_sdk.models.organisations_invite_sro_request import OrganisationsInviteSroRequest
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.OrganisationsApi(api_client)
    id = 1 # int | organisations entry ID
    organisations_invite_sro_request = safepeopleregistry_api_sdk.OrganisationsInviteSroRequest() # OrganisationsInviteSroRequest | 

    try:
        # organisations@inviteSro
        api_response = api_instance.organisations_invite_sro(id, organisations_invite_sro_request)
        print("The response of OrganisationsApi->organisations_invite_sro:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_invite_sro: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| organisations entry ID | 
 **organisations_invite_sro_request** | [**OrganisationsInviteSroRequest**](OrganisationsInviteSroRequest.md)|  | 

### Return type

[**OrganisationsInviteSro201Response**](OrganisationsInviteSro201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**400** | Invalid argument(s) |  -  |
**403** | Forbidden |  -  |
**409** | The email already belongs to a user; appoint an existing member with PUT /organisations/{id}/sro instead |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_remove_delegate**
> OrganisationsAppointSro200Response organisations_remove_delegate(id, user_id)

organisations@removeDelegate

Detaches a delegate from the organisation and notifies them and the remaining members. The SRO and delegates of the organisation can remove other delegates; the SRO cannot be removed and nobody can remove themselves.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisations_appoint_sro200_response import OrganisationsAppointSro200Response
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.OrganisationsApi(api_client)
    id = 1 # int | organisations entry ID
    user_id = 1 # int | ID of the delegate to remove

    try:
        # organisations@removeDelegate
        api_response = api_instance.organisations_remove_delegate(id, user_id)
        print("The response of OrganisationsApi->organisations_remove_delegate:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_remove_delegate: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| organisations entry ID | 
 **user_id** | **int**| ID of the delegate to remove | 

### Return type

[**OrganisationsAppointSro200Response**](OrganisationsAppointSro200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**403** | Forbidden |  -  |
**404** | The user is not a delegate of this organisation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_resend_sro_invite**
> OrganisationsAppointSro200Response organisations_resend_sro_invite(id)

organisations@resendSroInvite

Resends the pending SRO invitation with the code it already has. Delegates can resend while the organisation has no claimed SRO; after that only the SRO can.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisations_appoint_sro200_response import OrganisationsAppointSro200Response
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.OrganisationsApi(api_client)
    id = 1 # int | organisations entry ID

    try:
        # organisations@resendSroInvite
        api_response = api_instance.organisations_resend_sro_invite(id)
        print("The response of OrganisationsApi->organisations_resend_sro_invite:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_resend_sro_invite: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| organisations entry ID | 

### Return type

[**OrganisationsAppointSro200Response**](OrganisationsAppointSro200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**403** | Forbidden |  -  |
**404** | The organisation has no pending SRO invitation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

