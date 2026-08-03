# safepeopleregistry_api_sdk.ProjectHasOrganisationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**project_has_organisation_show**](ProjectHasOrganisationApi.md#project_has_organisation_show) | **GET** /api/v1/project-organisations/{projectOrganisationId} | Get details of a project-organisation relationship


# **project_has_organisation_show**
> ProjectHasOrganisation project_has_organisation_show(project_organisation_id)

Get details of a project-organisation relationship

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_has_organisation import ProjectHasOrganisation
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
    api_instance = safepeopleregistry_api_sdk.ProjectHasOrganisationApi(api_client)
    project_organisation_id = 1 # int | ID of the project-organisation relationship

    try:
        # Get details of a project-organisation relationship
        api_response = api_instance.project_has_organisation_show(project_organisation_id)
        print("The response of ProjectHasOrganisationApi->project_has_organisation_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectHasOrganisationApi->project_has_organisation_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_organisation_id** | **int**| ID of the project-organisation relationship | 

### Return type

[**ProjectHasOrganisation**](ProjectHasOrganisation.md)

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
**404** | Project-organisation relationship not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

