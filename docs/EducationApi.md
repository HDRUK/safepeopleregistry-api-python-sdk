# safepeopleregistry_api_sdk.EducationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**education_destroy_by_registry_id**](EducationApi.md#education_destroy_by_registry_id) | **DELETE** /api/v1/registries/{registryId}/educations/{id} | Delete an education record
[**education_index_by_registry_id**](EducationApi.md#education_index_by_registry_id) | **GET** /api/v1/educations/registries/{registryId} | Get education records by registry ID
[**education_show_by_registry_id**](EducationApi.md#education_show_by_registry_id) | **GET** /api/v1/educations/{id}/registries/{registryId} | Get a specific education record by ID and registry ID
[**education_store_by_registry_id**](EducationApi.md#education_store_by_registry_id) | **POST** /api/v1/registries/{registryId}/educations | Create a new education record for a registry
[**education_update_by_registry_id**](EducationApi.md#education_update_by_registry_id) | **PUT** /api/v1/registries/{registryId}/educations/{id} | Update an existing education record


# **education_destroy_by_registry_id**
> EducationDestroyByRegistryId200Response education_destroy_by_registry_id(registry_id, id)

Delete an education record

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.education_destroy_by_registry_id200_response import EducationDestroyByRegistryId200Response
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
    api_instance = safepeopleregistry_api_sdk.EducationApi(api_client)
    registry_id = 1 # int | ID of the registry
    id = 1 # int | ID of the education record

    try:
        # Delete an education record
        api_response = api_instance.education_destroy_by_registry_id(registry_id, id)
        print("The response of EducationApi->education_destroy_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EducationApi->education_destroy_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| ID of the registry | 
 **id** | **int**| ID of the education record | 

### Return type

[**EducationDestroyByRegistryId200Response**](EducationDestroyByRegistryId200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Deleted |  -  |
**400** | Invalid argument(s) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **education_index_by_registry_id**
> List[Education] education_index_by_registry_id(registry_id)

Get education records by registry ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.education import Education
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
    api_instance = safepeopleregistry_api_sdk.EducationApi(api_client)
    registry_id = 1 # int | ID of the registry

    try:
        # Get education records by registry ID
        api_response = api_instance.education_index_by_registry_id(registry_id)
        print("The response of EducationApi->education_index_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EducationApi->education_index_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| ID of the registry | 

### Return type

[**List[Education]**](Education.md)

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **education_show_by_registry_id**
> Education education_show_by_registry_id(registry_id, id)

Get a specific education record by ID and registry ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.education import Education
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
    api_instance = safepeopleregistry_api_sdk.EducationApi(api_client)
    registry_id = 1 # int | ID of the registry
    id = 1 # int | ID of the education record

    try:
        # Get a specific education record by ID and registry ID
        api_response = api_instance.education_show_by_registry_id(registry_id, id)
        print("The response of EducationApi->education_show_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EducationApi->education_show_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| ID of the registry | 
 **id** | **int**| ID of the education record | 

### Return type

[**Education**](Education.md)

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
**404** | Education record not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **education_store_by_registry_id**
> AccreditationStoreByRegistryId201Response education_store_by_registry_id(registry_id, education)

Create a new education record for a registry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.education import Education
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
    api_instance = safepeopleregistry_api_sdk.EducationApi(api_client)
    registry_id = 1 # int | ID of the registry
    education = safepeopleregistry_api_sdk.Education() # Education | 

    try:
        # Create a new education record for a registry
        api_response = api_instance.education_store_by_registry_id(registry_id, education)
        print("The response of EducationApi->education_store_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EducationApi->education_store_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| ID of the registry | 
 **education** | [**Education**](Education.md)|  | 

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
**201** | Created |  -  |
**400** | Invalid argument(s) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **education_update_by_registry_id**
> Education education_update_by_registry_id(registry_id, id, education)

Update an existing education record

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.education import Education
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
    api_instance = safepeopleregistry_api_sdk.EducationApi(api_client)
    registry_id = 1 # int | ID of the registry
    id = 1 # int | ID of the education record
    education = safepeopleregistry_api_sdk.Education() # Education | 

    try:
        # Update an existing education record
        api_response = api_instance.education_update_by_registry_id(registry_id, id, education)
        print("The response of EducationApi->education_update_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EducationApi->education_update_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| ID of the registry | 
 **id** | **int**| ID of the education record | 
 **education** | [**Education**](Education.md)|  | 

### Return type

[**Education**](Education.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Updated |  -  |
**400** | Invalid argument(s) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

