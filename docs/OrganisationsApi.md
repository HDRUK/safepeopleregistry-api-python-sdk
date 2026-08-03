# safepeopleregistry_api_sdk.OrganisationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**custodian_project_organisations_get_status**](OrganisationsApi.md#custodian_project_organisations_get_status) | **GET** /api/v1/custodian_approvals/{custodianId}/project/{projectId}/organisation/{organisationId}/projectOrganisations/status | Get project organisation status
[**organisations_custodian_invite_user**](OrganisationsApi.md#organisations_custodian_invite_user) | **POST** /api/v1/organisations/{id}/custodian_invite_user | organisations@custodian_invite_user
[**organisations_destroy**](OrganisationsApi.md#organisations_destroy) | **DELETE** /api/v1/organisations/{id} | organisations@destroy
[**organisations_get_registries**](OrganisationsApi.md#organisations_get_registries) | **GET** /api/v1/organisations/{id}/registries | Get all registries for an organisation
[**organisations_get_status**](OrganisationsApi.md#organisations_get_status) | **GET** /api/v1/organisations/{id}/status | Get organisation status
[**organisations_idvt**](OrganisationsApi.md#organisations_idvt) | **GET** /api/v1/organisations/{id}/idvt | organisations@idvt
[**organisations_invite_user**](OrganisationsApi.md#organisations_invite_user) | **POST** /api/v1/organisations/{id}/invite_user | organisations@invite_user
[**organisations_show**](OrganisationsApi.md#organisations_show) | **GET** /api/v1/organisations/{id} | organisations@show
[**organisations_store**](OrganisationsApi.md#organisations_store) | **POST** /api/v1/organisations | organisations@store
[**organisations_update**](OrganisationsApi.md#organisations_update) | **PUT** /api/v1/organisations/{id} | organisations@update
[**organisations_update_approved**](OrganisationsApi.md#organisations_update_approved) | **PUT** /api/v1/organisations/{id}/approved | SuperAdmin update org system_approved flag


# **custodian_project_organisations_get_status**
> CustodianProjectOrganisationsGetStatus200Response custodian_project_organisations_get_status(custodian_id, project_id, organisation_id)

Get project organisation status

Retrieve the status of a project organisation for a specific custodian using custodianId, projectId, and organisationId.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_project_organisations_get_status200_response import CustodianProjectOrganisationsGetStatus200Response
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
    custodian_id = 1 # int | Custodian ID
    project_id = 10 # int | Project ID
    organisation_id = 5 # int | Organisation ID

    try:
        # Get project organisation status
        api_response = api_instance.custodian_project_organisations_get_status(custodian_id, project_id, organisation_id)
        print("The response of OrganisationsApi->custodian_project_organisations_get_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->custodian_project_organisations_get_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| Custodian ID | 
 **project_id** | **int**| Project ID | 
 **organisation_id** | **int**| Organisation ID | 

### Return type

[**CustodianProjectOrganisationsGetStatus200Response**](CustodianProjectOrganisationsGetStatus200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Organisation or custodian project organisation not found |  -  |
**500** | Server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_custodian_invite_user**
> AccreditationStoreByRegistryId201Response organisations_custodian_invite_user(id, organisations_invite_user_request)

organisations@custodian_invite_user

Invites a user to org

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.organisations_invite_user_request import OrganisationsInviteUserRequest
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
    organisations_invite_user_request = safepeopleregistry_api_sdk.OrganisationsInviteUserRequest() # OrganisationsInviteUserRequest | Invite definition

    try:
        # organisations@custodian_invite_user
        api_response = api_instance.organisations_custodian_invite_user(id, organisations_invite_user_request)
        print("The response of OrganisationsApi->organisations_custodian_invite_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_custodian_invite_user: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| organisations entry ID | 
 **organisations_invite_user_request** | [**OrganisationsInviteUserRequest**](OrganisationsInviteUserRequest.md)| Invite definition | 

### Return type

[**AccreditationStoreByRegistryId201Response**](AccreditationStoreByRegistryId201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_destroy**
> AffiliationDestroy200Response organisations_destroy(id)

organisations@destroy

Delete an organisations entry from the system

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.affiliation_destroy200_response import AffiliationDestroy200Response
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
        # organisations@destroy
        api_response = api_instance.organisations_destroy(id)
        print("The response of OrganisationsApi->organisations_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| organisations entry ID | 

### Return type

[**AffiliationDestroy200Response**](AffiliationDestroy200Response.md)

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
**404** | Not found response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_get_registries**
> OrganisationsGetRegistries200Response organisations_get_registries(id, show_pending=show_pending)

Get all registries for an organisation

Returns all registries associated with the specified organisation

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisations_get_registries200_response import OrganisationsGetRegistries200Response
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
    id = 56 # int | Organisation ID
    show_pending = True # bool | Include users with pending invitations (true/false) (optional)

    try:
        # Get all registries for an organisation
        api_response = api_instance.organisations_get_registries(id, show_pending=show_pending)
        print("The response of OrganisationsApi->organisations_get_registries:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_get_registries: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Organisation ID | 
 **show_pending** | **bool**| Include users with pending invitations (true/false) | [optional] 

### Return type

[**OrganisationsGetRegistries200Response**](OrganisationsGetRegistries200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |
**400** | Invalid argument(s) |  -  |
**404** | No registries found for this organisation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_get_status**
> CustodianProjectOrganisationsGetStatus200Response organisations_get_status(id)

Get organisation status

Returns the organisation with its model state and state

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_project_organisations_get_status200_response import CustodianProjectOrganisationsGetStatus200Response
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
    id = 1 # int | Organisation ID

    try:
        # Get organisation status
        api_response = api_instance.organisations_get_status(id)
        print("The response of OrganisationsApi->organisations_get_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_get_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Organisation ID | 

### Return type

[**CustodianProjectOrganisationsGetStatus200Response**](CustodianProjectOrganisationsGetStatus200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Organisation not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_idvt**
> OrganisationsIdvt200Response organisations_idvt(id)

organisations@idvt

Return an organisations idvt details by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisations_idvt200_response import OrganisationsIdvt200Response
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
        # organisations@idvt
        api_response = api_instance.organisations_idvt(id)
        print("The response of OrganisationsApi->organisations_idvt:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_idvt: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| organisations entry ID | 

### Return type

[**OrganisationsIdvt200Response**](OrganisationsIdvt200Response.md)

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
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_invite_user**
> AccreditationStoreByRegistryId201Response organisations_invite_user(id, organisations_invite_user_request)

organisations@invite_user

Invites a user to org

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.organisations_invite_user_request import OrganisationsInviteUserRequest
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
    organisations_invite_user_request = safepeopleregistry_api_sdk.OrganisationsInviteUserRequest() # OrganisationsInviteUserRequest | Invite definition

    try:
        # organisations@invite_user
        api_response = api_instance.organisations_invite_user(id, organisations_invite_user_request)
        print("The response of OrganisationsApi->organisations_invite_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_invite_user: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| organisations entry ID | 
 **organisations_invite_user_request** | [**OrganisationsInviteUserRequest**](OrganisationsInviteUserRequest.md)| Invite definition | 

### Return type

[**AccreditationStoreByRegistryId201Response**](AccreditationStoreByRegistryId201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**403** | forbidden |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_show**
> OrganisationIndex200Response organisations_show(id)

organisations@show

Return an organisations entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisation_index200_response import OrganisationIndex200Response
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
        # organisations@show
        api_response = api_instance.organisations_show(id)
        print("The response of OrganisationsApi->organisations_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| organisations entry ID | 

### Return type

[**OrganisationIndex200Response**](OrganisationIndex200Response.md)

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
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_store**
> IdentityStore201Response organisations_store(organisation)

organisations@store

Create a organisations entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.identity_store201_response import IdentityStore201Response
from safepeopleregistry_api_sdk.models.organisation import Organisation
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
    organisation = safepeopleregistry_api_sdk.Organisation() # Organisation | organisations definition

    try:
        # organisations@store
        api_response = api_instance.organisations_store(organisation)
        print("The response of OrganisationsApi->organisations_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organisation** | [**Organisation**](Organisation.md)| organisations definition | 

### Return type

[**IdentityStore201Response**](IdentityStore201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**201** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_update**
> OrganisationsUpdate200Response organisations_update(id, organisation)

organisations@update

Update a organisations entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisation import Organisation
from safepeopleregistry_api_sdk.models.organisations_update200_response import OrganisationsUpdate200Response
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
    organisation = safepeopleregistry_api_sdk.Organisation() # Organisation | organisations definition

    try:
        # organisations@update
        api_response = api_instance.organisations_update(id, organisation)
        print("The response of OrganisationsApi->organisations_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| organisations entry ID | 
 **organisation** | [**Organisation**](Organisation.md)| organisations definition | 

### Return type

[**OrganisationsUpdate200Response**](OrganisationsUpdate200Response.md)

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
**404** | Not found response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **organisations_update_approved**
> AccreditationStoreByRegistryId201Response organisations_update_approved(id, organisations_update_approved_request)

SuperAdmin update org system_approved flag

Updates the system_approved flag for an organisation

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.organisations_update_approved_request import OrganisationsUpdateApprovedRequest
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
    organisations_update_approved_request = safepeopleregistry_api_sdk.OrganisationsUpdateApprovedRequest() # OrganisationsUpdateApprovedRequest | System approval update definition

    try:
        # SuperAdmin update org system_approved flag
        api_response = api_instance.organisations_update_approved(id, organisations_update_approved_request)
        print("The response of OrganisationsApi->organisations_update_approved:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationsApi->organisations_update_approved: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| organisations entry ID | 
 **organisations_update_approved_request** | [**OrganisationsUpdateApprovedRequest**](OrganisationsUpdateApprovedRequest.md)| System approval update definition | 

### Return type

[**AccreditationStoreByRegistryId201Response**](AccreditationStoreByRegistryId201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

