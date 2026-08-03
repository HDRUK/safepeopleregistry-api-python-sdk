# safepeopleregistry_api_sdk.InfringementApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**infringement_index**](InfringementApi.md#infringement_index) | **GET** /api/v1/infringements | Infringement@index
[**infringement_show**](InfringementApi.md#infringement_show) | **GET** /api/v1/infringements/{id} | Infringement@show
[**infringement_store**](InfringementApi.md#infringement_store) | **POST** /api/v1/infringements | Infringement@store


# **infringement_index**
> InfringementIndex200Response infringement_index()

Infringement@index

Return a list of Infringements

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.infringement_index200_response import InfringementIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.InfringementApi(api_client)

    try:
        # Infringement@index
        api_response = api_instance.infringement_index()
        print("The response of InfringementApi->infringement_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InfringementApi->infringement_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**InfringementIndex200Response**](InfringementIndex200Response.md)

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

# **infringement_show**
> InfringementIndex200Response infringement_show(id)

Infringement@show

Return an Infringement entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.infringement_index200_response import InfringementIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.InfringementApi(api_client)
    id = 1 # int | Infringement entry ID

    try:
        # Infringement@show
        api_response = api_instance.infringement_show(id)
        print("The response of InfringementApi->infringement_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InfringementApi->infringement_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Infringement entry ID | 

### Return type

[**InfringementIndex200Response**](InfringementIndex200Response.md)

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

# **infringement_store**
> InfringementStore201Response infringement_store(infringement_store_request)

Infringement@store

Create an Infringement entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.infringement_store201_response import InfringementStore201Response
from safepeopleregistry_api_sdk.models.infringement_store_request import InfringementStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.InfringementApi(api_client)
    infringement_store_request = safepeopleregistry_api_sdk.InfringementStoreRequest() # InfringementStoreRequest | Infringement definition

    try:
        # Infringement@store
        api_response = api_instance.infringement_store(infringement_store_request)
        print("The response of InfringementApi->infringement_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InfringementApi->infringement_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **infringement_store_request** | [**InfringementStoreRequest**](InfringementStoreRequest.md)| Infringement definition | 

### Return type

[**InfringementStore201Response**](InfringementStore201Response.md)

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

