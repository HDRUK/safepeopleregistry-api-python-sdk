# safepeopleregistry_api_sdk.ResolutionApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**resolution_index_by_registry_id**](ResolutionApi.md#resolution_index_by_registry_id) | **GET** /api/v1/registries/{registryId}/resolutions | Get resolutions by registry ID
[**resolution_store_by_registry_id**](ResolutionApi.md#resolution_store_by_registry_id) | **POST** /api/v1/registries/{registryId}/resolutions | Create a new resolution for a registry


# **resolution_index_by_registry_id**
> List[Resolution] resolution_index_by_registry_id(registry_id)

Get resolutions by registry ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.resolution import Resolution
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
    api_instance = safepeopleregistry_api_sdk.ResolutionApi(api_client)
    registry_id = 1 # int | ID of the registry

    try:
        # Get resolutions by registry ID
        api_response = api_instance.resolution_index_by_registry_id(registry_id)
        print("The response of ResolutionApi->resolution_index_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ResolutionApi->resolution_index_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| ID of the registry | 

### Return type

[**List[Resolution]**](Resolution.md)

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

# **resolution_store_by_registry_id**
> AccreditationStoreByRegistryId201Response resolution_store_by_registry_id(registry_id, resolution)

Create a new resolution for a registry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.resolution import Resolution
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
    api_instance = safepeopleregistry_api_sdk.ResolutionApi(api_client)
    registry_id = 1 # int | ID of the registry
    resolution = safepeopleregistry_api_sdk.Resolution() # Resolution | 

    try:
        # Create a new resolution for a registry
        api_response = api_instance.resolution_store_by_registry_id(registry_id, resolution)
        print("The response of ResolutionApi->resolution_store_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ResolutionApi->resolution_store_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| ID of the registry | 
 **resolution** | [**Resolution**](Resolution.md)|  | 

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

