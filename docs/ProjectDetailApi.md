# safepeopleregistry_api_sdk.ProjectDetailApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**project_detail_index**](ProjectDetailApi.md#project_detail_index) | **GET** /api/v1/project_details | ProjectDetail@index
[**project_detail_show**](ProjectDetailApi.md#project_detail_show) | **GET** /api/v1/project_details/{id} | ProjectDetail@show


# **project_detail_index**
> ProjectDetailIndex200Response project_detail_index()

ProjectDetail@index

Return a list of ProjectDetail

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_detail_index200_response import ProjectDetailIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectDetailApi(api_client)

    try:
        # ProjectDetail@index
        api_response = api_instance.project_detail_index()
        print("The response of ProjectDetailApi->project_detail_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectDetailApi->project_detail_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ProjectDetailIndex200Response**](ProjectDetailIndex200Response.md)

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

# **project_detail_show**
> ProjectDetailIndex200Response project_detail_show(id)

ProjectDetail@show

Return a ProjectDetail

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_detail_index200_response import ProjectDetailIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectDetailApi(api_client)
    id = 1 # int | ProjectDetail entry ID

    try:
        # ProjectDetail@show
        api_response = api_instance.project_detail_show(id)
        print("The response of ProjectDetailApi->project_detail_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectDetailApi->project_detail_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ProjectDetail entry ID | 

### Return type

[**ProjectDetailIndex200Response**](ProjectDetailIndex200Response.md)

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

