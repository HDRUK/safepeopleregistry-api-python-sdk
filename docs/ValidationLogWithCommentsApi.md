# safepeopleregistry_api_sdk.ValidationLogWithCommentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**validation_log_with_comments_index**](ValidationLogWithCommentsApi.md#validation_log_with_comments_index) | **GET** /api/v1/validation_logs/{id} | Get  a Validation Log


# **validation_log_with_comments_index**
> List[ValidationLog] validation_log_with_comments_index(id)

Get  a Validation Log

Retrieve a specific entry for a validation log .

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_log import ValidationLog
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
    api_instance = safepeopleregistry_api_sdk.ValidationLogWithCommentsApi(api_client)
    id = 56 # int | The ID of the validation log

    try:
        # Get  a Validation Log
        api_response = api_instance.validation_log_with_comments_index(id)
        print("The response of ValidationLogWithCommentsApi->validation_log_with_comments_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationLogWithCommentsApi->validation_log_with_comments_index: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| The ID of the validation log | 

### Return type

[**List[ValidationLog]**](ValidationLog.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Validation log with comments |  -  |
**404** | Validation log not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

