# safepeopleregistry_api_sdk.PermissionApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**permission_destroy**](PermissionApi.md#permission_destroy) | **DELETE** /api/v1/permissions/{id} | Permission@destroy
[**permission_index**](PermissionApi.md#permission_index) | **GET** /api/v1/permissions | Permission@index
[**permission_show**](PermissionApi.md#permission_show) | **GET** /api/v1/permissions/{id} | Permission@show
[**permission_store**](PermissionApi.md#permission_store) | **POST** /api/v1/permissions | Permission@store
[**permission_update**](PermissionApi.md#permission_update) | **PATCH** /api/v1/permissions/{id} | Permission@update


# **permission_destroy**
> AffiliationDestroy200Response permission_destroy(id)

Permission@destroy

Delete a Permission entry from the system

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
    api_instance = safepeopleregistry_api_sdk.PermissionApi(api_client)
    id = 1 # int | Permission entry ID

    try:
        # Permission@destroy
        api_response = api_instance.permission_destroy(id)
        print("The response of PermissionApi->permission_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PermissionApi->permission_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Permission entry ID | 

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
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **permission_index**
> PermissionIndex200Response permission_index()

Permission@index

Return a list of Permissions

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.permission_index200_response import PermissionIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.PermissionApi(api_client)

    try:
        # Permission@index
        api_response = api_instance.permission_index()
        print("The response of PermissionApi->permission_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PermissionApi->permission_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**PermissionIndex200Response**](PermissionIndex200Response.md)

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

# **permission_show**
> PermissionIndex200Response permission_show(id)

Permission@show

Return a Permission entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.permission_index200_response import PermissionIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.PermissionApi(api_client)
    id = 1 # int | Permission entry ID

    try:
        # Permission@show
        api_response = api_instance.permission_show(id)
        print("The response of PermissionApi->permission_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PermissionApi->permission_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Permission entry ID | 

### Return type

[**PermissionIndex200Response**](PermissionIndex200Response.md)

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

# **permission_store**
> AccreditationStoreByRegistryId201Response permission_store(permission_store_request)

Permission@store

Create a Permission entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.permission_store_request import PermissionStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.PermissionApi(api_client)
    permission_store_request = safepeopleregistry_api_sdk.PermissionStoreRequest() # PermissionStoreRequest | Permission definition

    try:
        # Permission@store
        api_response = api_instance.permission_store(permission_store_request)
        print("The response of PermissionApi->permission_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PermissionApi->permission_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **permission_store_request** | [**PermissionStoreRequest**](PermissionStoreRequest.md)| Permission definition | 

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
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **permission_update**
> PermissionUpdate200Response permission_update(id, permission_store_request)

Permission@update

Update a Permission entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.permission_store_request import PermissionStoreRequest
from safepeopleregistry_api_sdk.models.permission_update200_response import PermissionUpdate200Response
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
    api_instance = safepeopleregistry_api_sdk.PermissionApi(api_client)
    id = 1 # int | Permission entry ID
    permission_store_request = safepeopleregistry_api_sdk.PermissionStoreRequest() # PermissionStoreRequest | Permission definition

    try:
        # Permission@update
        api_response = api_instance.permission_update(id, permission_store_request)
        print("The response of PermissionApi->permission_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PermissionApi->permission_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Permission entry ID | 
 **permission_store_request** | [**PermissionStoreRequest**](PermissionStoreRequest.md)| Permission definition | 

### Return type

[**PermissionUpdate200Response**](PermissionUpdate200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

