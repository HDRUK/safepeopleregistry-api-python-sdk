# safepeopleregistry_api_sdk.ProjectUsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**project_users_bulk_invite_project_users**](ProjectUsersApi.md#project_users_bulk_invite_project_users) | **POST** /api/v1/project_users/bulk | Bulk invite Project Users


# **project_users_bulk_invite_project_users**
> project_users_bulk_invite_project_users(project_users_bulk_invite_project_users_request)

Bulk invite Project Users

Invite multiple users and attach them to a project

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_users_bulk_invite_project_users_request import ProjectUsersBulkInviteProjectUsersRequest
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
    api_instance = safepeopleregistry_api_sdk.ProjectUsersApi(api_client)
    project_users_bulk_invite_project_users_request = safepeopleregistry_api_sdk.ProjectUsersBulkInviteProjectUsersRequest() # ProjectUsersBulkInviteProjectUsersRequest | 

    try:
        # Bulk invite Project Users
        api_instance.project_users_bulk_invite_project_users(project_users_bulk_invite_project_users_request)
    except Exception as e:
        print("Exception when calling ProjectUsersApi->project_users_bulk_invite_project_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_users_bulk_invite_project_users_request** | [**ProjectUsersBulkInviteProjectUsersRequest**](ProjectUsersBulkInviteProjectUsersRequest.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

