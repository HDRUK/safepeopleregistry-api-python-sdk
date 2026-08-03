# safepeopleregistry_api_sdk.HistoryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**history_index**](HistoryApi.md#history_index) | **GET** /api/v1/histories | History@index
[**history_show**](HistoryApi.md#history_show) | **GET** /api/v1/histories/{id} | History@show
[**history_store**](HistoryApi.md#history_store) | **POST** /api/v1/histories | History@store


# **history_index**
> HistoryIndex200Response history_index()

History@index

Return a list of Histories

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.history_index200_response import HistoryIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.HistoryApi(api_client)

    try:
        # History@index
        api_response = api_instance.history_index()
        print("The response of HistoryApi->history_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling HistoryApi->history_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**HistoryIndex200Response**](HistoryIndex200Response.md)

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

# **history_show**
> HistoryIndex200Response history_show(id)

History@show

Return a History entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.history_index200_response import HistoryIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.HistoryApi(api_client)
    id = 1 # int | History entry ID

    try:
        # History@show
        api_response = api_instance.history_show(id)
        print("The response of HistoryApi->history_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling HistoryApi->history_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| History entry ID | 

### Return type

[**HistoryIndex200Response**](HistoryIndex200Response.md)

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

# **history_store**
> HistoryStore201Response history_store(history_store_request)

History@store

Create a History entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.history_store201_response import HistoryStore201Response
from safepeopleregistry_api_sdk.models.history_store_request import HistoryStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.HistoryApi(api_client)
    history_store_request = safepeopleregistry_api_sdk.HistoryStoreRequest() # HistoryStoreRequest | History definition

    try:
        # History@store
        api_response = api_instance.history_store(history_store_request)
        print("The response of HistoryApi->history_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling HistoryApi->history_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **history_store_request** | [**HistoryStoreRequest**](HistoryStoreRequest.md)| History definition | 

### Return type

[**HistoryStore201Response**](HistoryStore201Response.md)

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

