# safepeopleregistry_api_sdk.CustodianProjectOrganisationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**custodian_project_organisations_get_workflow_states**](CustodianProjectOrganisationsApi.md#custodian_project_organisations_get_workflow_states) | **GET** /api/v1/custodian_approvals/projectOrganisations/getWorkflowStates | Get all workflow states for custodian project organisation approvals
[**custodian_project_organisations_index**](CustodianProjectOrganisationsApi.md#custodian_project_organisations_index) | **GET** /api/v1/custodian_approvals/{custodianId}/projectOrganisations | List all project organisations associated with a custodian
[**custodian_project_organisations_show**](CustodianProjectOrganisationsApi.md#custodian_project_organisations_show) | **GET** /api/v1/custodian_approvals/{custodianId}/projectOrganisations/{projectOrganisationId} | Get custodian approval for a project organisation
[**custodian_project_organisations_update**](CustodianProjectOrganisationsApi.md#custodian_project_organisations_update) | **PUT** /api/v1/custodian_approvals/{custodianId}/projectOrganisations/{projectOrganisationId} | Update custodian approval for a project organisation


# **custodian_project_organisations_get_workflow_states**
> CustodianProjectOrganisationsGetWorkflowStates200Response custodian_project_organisations_get_workflow_states()

Get all workflow states for custodian project organisation approvals

Returns a list of all possible workflow states

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_project_organisations_get_workflow_states200_response import CustodianProjectOrganisationsGetWorkflowStates200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianProjectOrganisationsApi(api_client)

    try:
        # Get all workflow states for custodian project organisation approvals
        api_response = api_instance.custodian_project_organisations_get_workflow_states()
        print("The response of CustodianProjectOrganisationsApi->custodian_project_organisations_get_workflow_states:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianProjectOrganisationsApi->custodian_project_organisations_get_workflow_states: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CustodianProjectOrganisationsGetWorkflowStates200Response**](CustodianProjectOrganisationsGetWorkflowStates200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_project_organisations_index**
> CustodianProjectOrganisationsIndex200Response custodian_project_organisations_index(custodian_id)

List all project organisations associated with a custodian

Returns a list of all custodian project organisation approvals for a specific custodian

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_project_organisations_index200_response import CustodianProjectOrganisationsIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianProjectOrganisationsApi(api_client)
    custodian_id = 56 # int | ID of the custodian

    try:
        # List all project organisations associated with a custodian
        api_response = api_instance.custodian_project_organisations_index(custodian_id)
        print("The response of CustodianProjectOrganisationsApi->custodian_project_organisations_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianProjectOrganisationsApi->custodian_project_organisations_index: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 

### Return type

[**CustodianProjectOrganisationsIndex200Response**](CustodianProjectOrganisationsIndex200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |
**400** | Invalid argument(s) |  -  |
**403** | Forbidden |  -  |
**404** | Custodian Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_project_organisations_show**
> CustodianProjectOrganisationsShow200Response custodian_project_organisations_show(custodian_id, project_organisation_id)

Get custodian approval for a project organisation

Returns custodian approval details for a specific project organisation

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_project_organisations_show200_response import CustodianProjectOrganisationsShow200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianProjectOrganisationsApi(api_client)
    custodian_id = 56 # int | ID of the custodian
    project_organisation_id = 56 # int | ID of the project organisation

    try:
        # Get custodian approval for a project organisation
        api_response = api_instance.custodian_project_organisations_show(custodian_id, project_organisation_id)
        print("The response of CustodianProjectOrganisationsApi->custodian_project_organisations_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianProjectOrganisationsApi->custodian_project_organisations_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 
 **project_organisation_id** | **int**| ID of the project organisation | 

### Return type

[**CustodianProjectOrganisationsShow200Response**](CustodianProjectOrganisationsShow200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |
**400** | Invalid argument(s) |  -  |
**403** | Forbidden |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_project_organisations_update**
> CustodianProjectOrganisationsShow200Response custodian_project_organisations_update(custodian_id, project_organisation_id, custodian_project_organisations_update_request)

Update custodian approval for a project organisation

Updates approval status and/or comment for a project organisation

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_project_organisations_show200_response import CustodianProjectOrganisationsShow200Response
from safepeopleregistry_api_sdk.models.custodian_project_organisations_update_request import CustodianProjectOrganisationsUpdateRequest
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
    api_instance = safepeopleregistry_api_sdk.CustodianProjectOrganisationsApi(api_client)
    custodian_id = 56 # int | ID of the custodian
    project_organisation_id = 56 # int | ID of the project organisation
    custodian_project_organisations_update_request = safepeopleregistry_api_sdk.CustodianProjectOrganisationsUpdateRequest() # CustodianProjectOrganisationsUpdateRequest | 

    try:
        # Update custodian approval for a project organisation
        api_response = api_instance.custodian_project_organisations_update(custodian_id, project_organisation_id, custodian_project_organisations_update_request)
        print("The response of CustodianProjectOrganisationsApi->custodian_project_organisations_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianProjectOrganisationsApi->custodian_project_organisations_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 
 **project_organisation_id** | **int**| ID of the project organisation | 
 **custodian_project_organisations_update_request** | [**CustodianProjectOrganisationsUpdateRequest**](CustodianProjectOrganisationsUpdateRequest.md)|  | 

### Return type

[**CustodianProjectOrganisationsShow200Response**](CustodianProjectOrganisationsShow200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |
**400** | Invalid argument(s) |  -  |
**403** | Forbidden |  -  |
**404** | Not Found |  -  |
**500** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

