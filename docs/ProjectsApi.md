# safepeopleregistry_api_sdk.ProjectsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**projects_delete**](ProjectsApi.md#projects_delete) | **DELETE** /api/v1/project_users/{id} | ProjectHasUser@delete
[**projects_get_validated_projects**](ProjectsApi.md#projects_get_validated_projects) | **GET** /api/v1/projects/user/{registryId}/validated | Project@getValidatedProjects


# **projects_delete**
> projects_delete(id)

ProjectHasUser@delete

Delete a user from a project

### Example


```python
import safepeopleregistry_api_sdk
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
    api_instance = safepeopleregistry_api_sdk.ProjectsApi(api_client)
    id = 1 # int | ID

    try:
        # ProjectHasUser@delete
        api_instance.projects_delete(id)
    except Exception as e:
        print("Exception when calling ProjectsApi->projects_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | success |  -  |
**400** | Invalid argument(s) |  -  |
**404** | failed |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **projects_get_validated_projects**
> OrganisationGetProjects200Response projects_get_validated_projects(registry_id)

Project@getValidatedProjects

Return (approved) projects for a registry (user)

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisation_get_projects200_response import OrganisationGetProjects200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectsApi(api_client)
    registry_id = 1 # int | Registry ID

    try:
        # Project@getValidatedProjects
        api_response = api_instance.projects_get_validated_projects(registry_id)
        print("The response of ProjectsApi->projects_get_validated_projects:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->projects_get_validated_projects: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **registry_id** | **int**| Registry ID | 

### Return type

[**OrganisationGetProjects200Response**](OrganisationGetProjects200Response.md)

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

