# safepeopleregistry_api_sdk.ActionLogsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**action_logs_get_entity_action_log**](ActionLogsApi.md#action_logs_get_entity_action_log) | **GET** /api/v1/{entity}/{id}/action_log | Get Action Logs for an Entity
[**action_logs_update**](ActionLogsApi.md#action_logs_update) | **PUT** /api/v1/action_logs/{id} | Update an Action Log


# **action_logs_get_entity_action_log**
> ActionLogsGetEntityActionLog200Response action_logs_get_entity_action_log(entity, id)

Get Action Logs for an Entity

Retrieve action logs for a given entity type (users, organisations) by ID.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.action_logs_get_entity_action_log200_response import ActionLogsGetEntityActionLog200Response
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
    api_instance = safepeopleregistry_api_sdk.ActionLogsApi(api_client)
    entity = 'entity_example' # str | The entity type (e.g., users, organisations)
    id = 56 # int | The ID of the entity

    try:
        # Get Action Logs for an Entity
        api_response = api_instance.action_logs_get_entity_action_log(entity, id)
        print("The response of ActionLogsApi->action_logs_get_entity_action_log:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ActionLogsApi->action_logs_get_entity_action_log: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **entity** | **str**| The entity type (e.g., users, organisations) | 
 **id** | **int**| The ID of the entity | 

### Return type

[**ActionLogsGetEntityActionLog200Response**](ActionLogsGetEntityActionLog200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response with action logs |  -  |
**404** | No action logs found for this entity |  -  |
**400** | Invalid entity type |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **action_logs_update**
> ActionLogsUpdate200Response action_logs_update(id, complete=complete, incomplete=incomplete)

Update an Action Log

Update an action log entry, including marking it as complete or incomplete.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.action_logs_update200_response import ActionLogsUpdate200Response
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
    api_instance = safepeopleregistry_api_sdk.ActionLogsApi(api_client)
    id = 56 # int | ID of the action log
    complete = True # bool | Mark as complete (optional)
    incomplete = True # bool | Mark as incomplete (optional)

    try:
        # Update an Action Log
        api_response = api_instance.action_logs_update(id, complete=complete, incomplete=incomplete)
        print("The response of ActionLogsApi->action_logs_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ActionLogsApi->action_logs_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the action log | 
 **complete** | **bool**| Mark as complete | [optional] 
 **incomplete** | **bool**| Mark as incomplete | [optional] 

### Return type

[**ActionLogsUpdate200Response**](ActionLogsUpdate200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Action status updated successfully |  -  |
**404** | Action log not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

