# safepeopleregistry_api_sdk.AccreditationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**accreditation_index_by_registry_id**](AccreditationApi.md#accreditation_index_by_registry_id) | **GET** /api/v1/accreditations/{registryId} | Get accreditations by registry ID
[**accreditation_store_by_registry_id**](AccreditationApi.md#accreditation_store_by_registry_id) | **POST** /api/v1/accreditations/{registryId} | Create accreditation for a registry
[**accreditation_update_by_registry_id**](AccreditationApi.md#accreditation_update_by_registry_id) | **PUT** /api/v1/accreditations/{id}/registries/{registryId} | Update accreditation for a registry


# **accreditation_index_by_registry_id**
> AccreditationIndexByRegistryId200Response accreditation_index_by_registry_id(registry_id)

Get accreditations by registry ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_index_by_registry_id200_response import AccreditationIndexByRegistryId200Response
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
    api_instance = safepeopleregistry_api_sdk.AccreditationApi(api_client)
    registry_id = 1 # int | ID of the registry

    try:
        # Get accreditations by registry ID
        api_response = api_instance.accreditation_index_by_registry_id(registry_id)
        print("The response of AccreditationApi->accreditation_index_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccreditationApi->accreditation_index_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| ID of the registry | 

### Return type

[**AccreditationIndexByRegistryId200Response**](AccreditationIndexByRegistryId200Response.md)

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

# **accreditation_store_by_registry_id**
> AccreditationStoreByRegistryId201Response accreditation_store_by_registry_id(registry_id, accreditation)

Create accreditation for a registry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation import Accreditation
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
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
    api_instance = safepeopleregistry_api_sdk.AccreditationApi(api_client)
    registry_id = 1 # int | ID of the registry
    accreditation = safepeopleregistry_api_sdk.Accreditation() # Accreditation | 

    try:
        # Create accreditation for a registry
        api_response = api_instance.accreditation_store_by_registry_id(registry_id, accreditation)
        print("The response of AccreditationApi->accreditation_store_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccreditationApi->accreditation_store_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| ID of the registry | 
 **accreditation** | [**Accreditation**](Accreditation.md)|  | 

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

# **accreditation_update_by_registry_id**
> AccreditationUpdateByRegistryId200Response accreditation_update_by_registry_id(registry_id, id, accreditation)

Update accreditation for a registry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation import Accreditation
from safepeopleregistry_api_sdk.models.accreditation_update_by_registry_id200_response import AccreditationUpdateByRegistryId200Response
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
    api_instance = safepeopleregistry_api_sdk.AccreditationApi(api_client)
    registry_id = 1 # int | ID of the registry
    id = 1 # int | ID of the accreditation
    accreditation = safepeopleregistry_api_sdk.Accreditation() # Accreditation | 

    try:
        # Update accreditation for a registry
        api_response = api_instance.accreditation_update_by_registry_id(registry_id, id, accreditation)
        print("The response of AccreditationApi->accreditation_update_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AccreditationApi->accreditation_update_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| ID of the registry | 
 **id** | **int**| ID of the accreditation | 
 **accreditation** | [**Accreditation**](Accreditation.md)|  | 

### Return type

[**AccreditationUpdateByRegistryId200Response**](AccreditationUpdateByRegistryId200Response.md)

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

