# safepeopleregistry_api_sdk.FilesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**files_download**](FilesApi.md#files_download) | **GET** /api/v1/files/{id}/download | Download an uploaded file
[**files_show**](FilesApi.md#files_show) | **GET** /api/v1/files/{id} | Files@show
[**files_store**](FilesApi.md#files_store) | **POST** /api/v1/files | Files@store


# **files_download**
> bytes files_download(id)

Download an uploaded file

Downloads the specified file

### Example


```python
import safepeopleregistry_api_sdk
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
    api_instance = safepeopleregistry_api_sdk.FilesApi(api_client)
    id = 1 # int | File ID

    try:
        # Download an uploaded file
        api_response = api_instance.files_download(id)
        print("The response of FilesApi->files_download:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->files_download: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| File ID | 

### Return type

**bytes**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/octet-stream, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | File downloaded successfully |  -  |
**400** | Invalid argument(s) |  -  |
**404** | File not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **files_show**
> FilesShow200Response files_show(id)

Files@show

Gets an uploaded file

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.files_show200_response import FilesShow200Response
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
    api_instance = safepeopleregistry_api_sdk.FilesApi(api_client)
    id = 1 # int | File ID

    try:
        # Files@show
        api_response = api_instance.files_show(id)
        print("The response of FilesApi->files_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->files_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| File ID | 

### Return type

[**FilesShow200Response**](FilesShow200Response.md)

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
**404** | Not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **files_store**
> AccreditationStoreByRegistryId201Response files_store(registry_id=registry_id, file=file, file_type=file_type, entity_type=entity_type)

Files@store

Uploads a file to the registry

### Example


```python
import safepeopleregistry_api_sdk
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
    api_instance = safepeopleregistry_api_sdk.FilesApi(api_client)
    registry_id = 56 # int |  (optional)
    file = None # bytes |  (optional)
    file_type = 'file_type_example' # str |  (optional)
    entity_type = 'entity_type_example' # str |  (optional)

    try:
        # Files@store
        api_response = api_instance.files_store(registry_id=registry_id, file=file, file_type=file_type, entity_type=entity_type)
        print("The response of FilesApi->files_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FilesApi->files_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**|  | [optional] 
 **file** | **bytes**|  | [optional] 
 **file_type** | **str**|  | [optional] 
 **entity_type** | **str**|  | [optional] 

### Return type

[**AccreditationStoreByRegistryId201Response**](AccreditationStoreByRegistryId201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Bad request |  -  |
**201** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

