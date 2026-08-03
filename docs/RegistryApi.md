# safepeopleregistry_api_sdk.RegistryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**registry_destroy**](RegistryApi.md#registry_destroy) | **DELETE** /api/v1/registry/{id} | Registry@destroy
[**registry_index**](RegistryApi.md#registry_index) | **GET** /api/v1/registry | Registry@index
[**registry_show**](RegistryApi.md#registry_show) | **GET** /api/v1/registry/{id} | Registry@show
[**registry_store**](RegistryApi.md#registry_store) | **POST** /api/v1/registry | Registry@store
[**registry_update**](RegistryApi.md#registry_update) | **PUT** /api/v1/registry/{id} | Registry@update


# **registry_destroy**
> AffiliationDestroy200Response registry_destroy(id)

Registry@destroy

Delete a Registry entry from the system

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
    api_instance = safepeopleregistry_api_sdk.RegistryApi(api_client)
    id = 1 # int | Registry entry ID

    try:
        # Registry@destroy
        api_response = api_instance.registry_destroy(id)
        print("The response of RegistryApi->registry_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistryApi->registry_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Registry entry ID | 

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

# **registry_index**
> RegistryIndex200Response registry_index()

Registry@index

Return a list of Registry entries

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.registry_index200_response import RegistryIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.RegistryApi(api_client)

    try:
        # Registry@index
        api_response = api_instance.registry_index()
        print("The response of RegistryApi->registry_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistryApi->registry_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**RegistryIndex200Response**](RegistryIndex200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registry_show**
> RegistryIndex200Response registry_show(id)

Registry@show

Return a Registry entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.registry_index200_response import RegistryIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.RegistryApi(api_client)
    id = 1 # int | Registry entry ID

    try:
        # Registry@show
        api_response = api_instance.registry_show(id)
        print("The response of RegistryApi->registry_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistryApi->registry_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Registry entry ID | 

### Return type

[**RegistryIndex200Response**](RegistryIndex200Response.md)

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

# **registry_store**
> AccreditationStoreByRegistryId201Response registry_store(registry)

Registry@store

Create a Registry entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.registry import Registry
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
    api_instance = safepeopleregistry_api_sdk.RegistryApi(api_client)
    registry = safepeopleregistry_api_sdk.Registry() # Registry | Registry definition

    try:
        # Registry@store
        api_response = api_instance.registry_store(registry)
        print("The response of RegistryApi->registry_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistryApi->registry_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry** | [**Registry**](Registry.md)| Registry definition | 

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
**404** | Not found response |  -  |
**201** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **registry_update**
> RegistryUpdate200Response registry_update(id, registry)

Registry@update

Update a Registry entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.registry import Registry
from safepeopleregistry_api_sdk.models.registry_update200_response import RegistryUpdate200Response
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
    api_instance = safepeopleregistry_api_sdk.RegistryApi(api_client)
    id = 1 # int | Registry entry ID
    registry = safepeopleregistry_api_sdk.Registry() # Registry | Registry definition

    try:
        # Registry@update
        api_response = api_instance.registry_update(id, registry)
        print("The response of RegistryApi->registry_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RegistryApi->registry_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Registry entry ID | 
 **registry** | [**Registry**](Registry.md)| Registry definition | 

### Return type

[**RegistryUpdate200Response**](RegistryUpdate200Response.md)

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

