# safepeopleregistry_api_sdk.ValidationLogCommentsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**validation_log_comments_comments**](ValidationLogCommentsApi.md#validation_log_comments_comments) | **GET** /api/v1/validation_logs/{id}/comments | Get all comments for a Validation Log
[**validation_log_comments_destroy**](ValidationLogCommentsApi.md#validation_log_comments_destroy) | **DELETE** /api/v1/validation_log_comments/{id} | Delete a validation log comment
[**validation_log_comments_show**](ValidationLogCommentsApi.md#validation_log_comments_show) | **GET** /api/v1/validation_log_comments/{id} | Get a single validation log comment
[**validation_log_comments_store**](ValidationLogCommentsApi.md#validation_log_comments_store) | **POST** /api/v1/validation_log_comments | Create a new validation log comment
[**validation_log_comments_update**](ValidationLogCommentsApi.md#validation_log_comments_update) | **PUT** /api/v1/validation_log_comments/{id} | Update a validation log comment


# **validation_log_comments_comments**
> List[ValidationLog] validation_log_comments_comments(id)

Get all comments for a Validation Log

Retrieve all comments associated with a specific validation log entry.

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
    api_instance = safepeopleregistry_api_sdk.ValidationLogCommentsApi(api_client)
    id = 56 # int | The ID of the validation log

    try:
        # Get all comments for a Validation Log
        api_response = api_instance.validation_log_comments_comments(id)
        print("The response of ValidationLogCommentsApi->validation_log_comments_comments:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationLogCommentsApi->validation_log_comments_comments: %s\n" % e)
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

# **validation_log_comments_destroy**
> ValidationLogCommentsDestroy200Response validation_log_comments_destroy(id)

Delete a validation log comment

Remove a comment from the validation logs.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_log_comments_destroy200_response import ValidationLogCommentsDestroy200Response
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
    api_instance = safepeopleregistry_api_sdk.ValidationLogCommentsApi(api_client)
    id = 56 # int | The ID of the comment

    try:
        # Delete a validation log comment
        api_response = api_instance.validation_log_comments_destroy(id)
        print("The response of ValidationLogCommentsApi->validation_log_comments_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationLogCommentsApi->validation_log_comments_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| The ID of the comment | 

### Return type

[**ValidationLogCommentsDestroy200Response**](ValidationLogCommentsDestroy200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Comment deleted successfully |  -  |
**400** | Comment not found |  -  |
**404** | Comment not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validation_log_comments_show**
> ValidationLogComment validation_log_comments_show(id)

Get a single validation log comment

Retrieve a specific validation log comment by ID.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_log_comment import ValidationLogComment
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
    api_instance = safepeopleregistry_api_sdk.ValidationLogCommentsApi(api_client)
    id = 56 # int | The ID of the comment

    try:
        # Get a single validation log comment
        api_response = api_instance.validation_log_comments_show(id)
        print("The response of ValidationLogCommentsApi->validation_log_comments_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationLogCommentsApi->validation_log_comments_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| The ID of the comment | 

### Return type

[**ValidationLogComment**](ValidationLogComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Comment retrieved successfully |  -  |
**400** | Comment not found |  -  |
**404** | Comment not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validation_log_comments_store**
> ValidationLogComment validation_log_comments_store(validation_log_comments_store_request)

Create a new validation log comment

Add a new comment to a validation log.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_log_comment import ValidationLogComment
from safepeopleregistry_api_sdk.models.validation_log_comments_store_request import ValidationLogCommentsStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.ValidationLogCommentsApi(api_client)
    validation_log_comments_store_request = safepeopleregistry_api_sdk.ValidationLogCommentsStoreRequest() # ValidationLogCommentsStoreRequest | 

    try:
        # Create a new validation log comment
        api_response = api_instance.validation_log_comments_store(validation_log_comments_store_request)
        print("The response of ValidationLogCommentsApi->validation_log_comments_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationLogCommentsApi->validation_log_comments_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **validation_log_comments_store_request** | [**ValidationLogCommentsStoreRequest**](ValidationLogCommentsStoreRequest.md)|  | 

### Return type

[**ValidationLogComment**](ValidationLogComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Comment created successfully |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validation_log_comments_update**
> ValidationLogComment validation_log_comments_update(id, validation_log_comments_update_request)

Update a validation log comment

Edit an existing validation log comment.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_log_comment import ValidationLogComment
from safepeopleregistry_api_sdk.models.validation_log_comments_update_request import ValidationLogCommentsUpdateRequest
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
    api_instance = safepeopleregistry_api_sdk.ValidationLogCommentsApi(api_client)
    id = 56 # int | The ID of the comment
    validation_log_comments_update_request = safepeopleregistry_api_sdk.ValidationLogCommentsUpdateRequest() # ValidationLogCommentsUpdateRequest | 

    try:
        # Update a validation log comment
        api_response = api_instance.validation_log_comments_update(id, validation_log_comments_update_request)
        print("The response of ValidationLogCommentsApi->validation_log_comments_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationLogCommentsApi->validation_log_comments_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| The ID of the comment | 
 **validation_log_comments_update_request** | [**ValidationLogCommentsUpdateRequest**](ValidationLogCommentsUpdateRequest.md)|  | 

### Return type

[**ValidationLogComment**](ValidationLogComment.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Comment updated successfully |  -  |
**400** | Comment not found |  -  |
**404** | Comment not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

