# safepeopleregistry_api_sdk.QueryApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**query_query**](QueryApi.md#query_query) | **POST** /api/v1/query | Query@query


# **query_query**
> QueryQuery200Response query_query(x_client_id, query_query_request)

Query@query

Query the registry by Digital Identifier

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.query_query200_response import QueryQuery200Response
from safepeopleregistry_api_sdk.models.query_query_request import QueryQueryRequest
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
    api_instance = safepeopleregistry_api_sdk.QueryApi(api_client)
    x_client_id = '8f14e45f-ceea-467e-adc1-0000example' # str | Custodian client ID used to authenticate the requesting custodian
    query_query_request = safepeopleregistry_api_sdk.QueryQueryRequest() # QueryQueryRequest | Query definition

    try:
        # Query@query
        api_response = api_instance.query_query(x_client_id, query_query_request)
        print("The response of QueryApi->query_query:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling QueryApi->query_query: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_client_id** | **str**| Custodian client ID used to authenticate the requesting custodian | 
 **query_query_request** | [**QueryQueryRequest**](QueryQueryRequest.md)| Query definition | 

### Return type

[**QueryQuery200Response**](QueryQuery200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**401** | Unauthorised - missing or unrecognised x-client-id header |  -  |
**404** | Not found response |  -  |
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

