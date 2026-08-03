# safepeopleregistry_api_sdk.AffiliationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**affiliations_get_organisation_affiliation**](AffiliationsApi.md#affiliations_get_organisation_affiliation) | **GET** /api/v1/affiliations/{registryId}/organisation/{organisationId} | Return a specific organisation&#39;s affiliation by registry ID and organisation ID
[**affiliations_index_by_registry_id**](AffiliationsApi.md#affiliations_index_by_registry_id) | **GET** /api/v1/affiliations/{registryId} | Affiliations@show
[**affiliations_store_by_registry_id**](AffiliationsApi.md#affiliations_store_by_registry_id) | **POST** /api/v1/affiliations/{registryId} | Affiliations@store
[**affiliations_update**](AffiliationsApi.md#affiliations_update) | **PUT** /api/v1/affiliations/{id} | Affiliations@update
[**affiliations_verify_email**](AffiliationsApi.md#affiliations_verify_email) | **PUT** /api/v1/affiliations/verify_email/{verificationCode} | Affiliations@verifyEmail


# **affiliations_get_organisation_affiliation**
> AffiliationsGetOrganisationAffiliation200Response affiliations_get_organisation_affiliation(registry_id, organisation_id)

Return a specific organisation's affiliation by registry ID and organisation ID

Get a specific organisation's affiliation for a given registry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.affiliations_get_organisation_affiliation200_response import AffiliationsGetOrganisationAffiliation200Response
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
    api_instance = safepeopleregistry_api_sdk.AffiliationsApi(api_client)
    registry_id = 1 # int | Registry ID
    organisation_id = 100 # int | Organisation ID

    try:
        # Return a specific organisation's affiliation by registry ID and organisation ID
        api_response = api_instance.affiliations_get_organisation_affiliation(registry_id, organisation_id)
        print("The response of AffiliationsApi->affiliations_get_organisation_affiliation:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AffiliationsApi->affiliations_get_organisation_affiliation: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| Registry ID | 
 **organisation_id** | **int**| Organisation ID | 

### Return type

[**AffiliationsGetOrganisationAffiliation200Response**](AffiliationsGetOrganisationAffiliation200Response.md)

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
**404** | Affiliation not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **affiliations_index_by_registry_id**
> AffiliationsIndexByRegistryId200Response affiliations_index_by_registry_id(registry_id)

Affiliations@show

Return a list of affiliations by registry id

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.affiliations_index_by_registry_id200_response import AffiliationsIndexByRegistryId200Response
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
    api_instance = safepeopleregistry_api_sdk.AffiliationsApi(api_client)
    registry_id = 1 # int | Affiliations registry id

    try:
        # Affiliations@show
        api_response = api_instance.affiliations_index_by_registry_id(registry_id)
        print("The response of AffiliationsApi->affiliations_index_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AffiliationsApi->affiliations_index_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| Affiliations registry id | 

### Return type

[**AffiliationsIndexByRegistryId200Response**](AffiliationsIndexByRegistryId200Response.md)

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

# **affiliations_store_by_registry_id**
> AffiliationsStoreByRegistryId200Response affiliations_store_by_registry_id(registry_id, affiliation)

Affiliations@store

Create an Affiliation entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.affiliation import Affiliation
from safepeopleregistry_api_sdk.models.affiliations_store_by_registry_id200_response import AffiliationsStoreByRegistryId200Response
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
    api_instance = safepeopleregistry_api_sdk.AffiliationsApi(api_client)
    registry_id = 1 # int | Registry entry ID
    affiliation = safepeopleregistry_api_sdk.Affiliation() # Affiliation | Affiliation definition

    try:
        # Affiliations@store
        api_response = api_instance.affiliations_store_by_registry_id(registry_id, affiliation)
        print("The response of AffiliationsApi->affiliations_store_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AffiliationsApi->affiliations_store_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| Registry entry ID | 
 **affiliation** | [**Affiliation**](Affiliation.md)| Affiliation definition | 

### Return type

[**AffiliationsStoreByRegistryId200Response**](AffiliationsStoreByRegistryId200Response.md)

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

# **affiliations_update**
> AffiliationsStoreByRegistryId200Response affiliations_update(id, affiliation)

Affiliations@update

Update an Affiliation entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.affiliation import Affiliation
from safepeopleregistry_api_sdk.models.affiliations_store_by_registry_id200_response import AffiliationsStoreByRegistryId200Response
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
    api_instance = safepeopleregistry_api_sdk.AffiliationsApi(api_client)
    id = 1 # int | Affiliation entry ID
    affiliation = safepeopleregistry_api_sdk.Affiliation() # Affiliation | Affiliation definition

    try:
        # Affiliations@update
        api_response = api_instance.affiliations_update(id, affiliation)
        print("The response of AffiliationsApi->affiliations_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AffiliationsApi->affiliations_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Affiliation entry ID | 
 **affiliation** | [**Affiliation**](Affiliation.md)| Affiliation definition | 

### Return type

[**AffiliationsStoreByRegistryId200Response**](AffiliationsStoreByRegistryId200Response.md)

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

# **affiliations_verify_email**
> AffiliationsStoreByRegistryId200Response affiliations_verify_email(verification_code)

Affiliations@verifyEmail

Update an Affiliation entry with verification

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.affiliations_store_by_registry_id200_response import AffiliationsStoreByRegistryId200Response
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
    api_instance = safepeopleregistry_api_sdk.AffiliationsApi(api_client)
    verification_code = '1' # str | Email verification code

    try:
        # Affiliations@verifyEmail
        api_response = api_instance.affiliations_verify_email(verification_code)
        print("The response of AffiliationsApi->affiliations_verify_email:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AffiliationsApi->affiliations_verify_email: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **verification_code** | **str**| Email verification code | 

### Return type

[**AffiliationsStoreByRegistryId200Response**](AffiliationsStoreByRegistryId200Response.md)

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

