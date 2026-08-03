# safepeopleregistry_api_sdk.ValidationLogsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**validation_logs_get_custodian_organisation_validation_logs**](ValidationLogsApi.md#validation_logs_get_custodian_organisation_validation_logs) | **GET** /api/v1/custodians/{custodianId}/organisation/{organisationId}/validation_logs | Get Validation Logs for Custodian and Organisation
[**validation_logs_get_custodian_project_user_validation_logs**](ValidationLogsApi.md#validation_logs_get_custodian_project_user_validation_logs) | **GET** /api/v1/custodians/{custodianId}/projects/{projectId}/registries/{registryId}/validation_logs | Get Validation Logs for Custodian, Project, and Registry
[**validation_logs_update**](ValidationLogsApi.md#validation_logs_update) | **PUT** /api/v1/validation_logs/{id} | Update a Validation Log
[**validation_logs_update_custodian_validation_logs**](ValidationLogsApi.md#validation_logs_update_custodian_validation_logs) | **PUT** /api/v1/custodians/{custodianId}/validation_Logs | Enable or Disable All Validation Logs for a Custodian Across Projects/Registries


# **validation_logs_get_custodian_organisation_validation_logs**
> ValidationLogsGetCustodianProjectUserValidationLogs200Response validation_logs_get_custodian_organisation_validation_logs(custodian_id, organisation_id, show_disabled=show_disabled)

Get Validation Logs for Custodian and Organisation

Retrieve validation logs associated with a given custodian and organisation.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_logs_get_custodian_project_user_validation_logs200_response import ValidationLogsGetCustodianProjectUserValidationLogs200Response
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
    api_instance = safepeopleregistry_api_sdk.ValidationLogsApi(api_client)
    custodian_id = 56 # int | The ID of the custodian entity
    organisation_id = 56 # int | The ID of the organisation entity
    show_disabled = True # bool | Whether to include disabled validation logs (optional)

    try:
        # Get Validation Logs for Custodian and Organisation
        api_response = api_instance.validation_logs_get_custodian_organisation_validation_logs(custodian_id, organisation_id, show_disabled=show_disabled)
        print("The response of ValidationLogsApi->validation_logs_get_custodian_organisation_validation_logs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationLogsApi->validation_logs_get_custodian_organisation_validation_logs: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| The ID of the custodian entity | 
 **organisation_id** | **int**| The ID of the organisation entity | 
 **show_disabled** | **bool**| Whether to include disabled validation logs | [optional] 

### Return type

[**ValidationLogsGetCustodianProjectUserValidationLogs200Response**](ValidationLogsGetCustodianProjectUserValidationLogs200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response with validation logs |  -  |
**404** | Custodian or Organisation not found |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validation_logs_get_custodian_project_user_validation_logs**
> ValidationLogsGetCustodianProjectUserValidationLogs200Response validation_logs_get_custodian_project_user_validation_logs(custodian_id, project_id, registry_id)

Get Validation Logs for Custodian, Project, and Registry

Retrieve validation logs associated with a given custodian, project, and registry.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_logs_get_custodian_project_user_validation_logs200_response import ValidationLogsGetCustodianProjectUserValidationLogs200Response
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
    api_instance = safepeopleregistry_api_sdk.ValidationLogsApi(api_client)
    custodian_id = 56 # int | The ID of the custodian entity
    project_id = 56 # int | The ID of the project entity
    registry_id = 56 # int | The ID of the registry entity

    try:
        # Get Validation Logs for Custodian, Project, and Registry
        api_response = api_instance.validation_logs_get_custodian_project_user_validation_logs(custodian_id, project_id, registry_id)
        print("The response of ValidationLogsApi->validation_logs_get_custodian_project_user_validation_logs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationLogsApi->validation_logs_get_custodian_project_user_validation_logs: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| The ID of the custodian entity | 
 **project_id** | **int**| The ID of the project entity | 
 **registry_id** | **int**| The ID of the registry entity | 

### Return type

[**ValidationLogsGetCustodianProjectUserValidationLogs200Response**](ValidationLogsGetCustodianProjectUserValidationLogs200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response with validation logs |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validation_logs_update**
> ValidationLogsUpdate200Response validation_logs_update(id, validation_logs_update_request=validation_logs_update_request)

Update a Validation Log

Update a validation log entry, including marking it as complete, incomplete, passed, or failed.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_logs_update200_response import ValidationLogsUpdate200Response
from safepeopleregistry_api_sdk.models.validation_logs_update_request import ValidationLogsUpdateRequest
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
    api_instance = safepeopleregistry_api_sdk.ValidationLogsApi(api_client)
    id = 56 # int | The ID of the validation log entry
    validation_logs_update_request = safepeopleregistry_api_sdk.ValidationLogsUpdateRequest() # ValidationLogsUpdateRequest |  (optional)

    try:
        # Update a Validation Log
        api_response = api_instance.validation_logs_update(id, validation_logs_update_request=validation_logs_update_request)
        print("The response of ValidationLogsApi->validation_logs_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationLogsApi->validation_logs_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| The ID of the validation log entry | 
 **validation_logs_update_request** | [**ValidationLogsUpdateRequest**](ValidationLogsUpdateRequest.md)|  | [optional] 

### Return type

[**ValidationLogsUpdate200Response**](ValidationLogsUpdate200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Validation log status updated successfully |  -  |
**404** | Validation log not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validation_logs_update_custodian_validation_logs**
> ValidationLogsUpdateCustodianValidationLogs200Response validation_logs_update_custodian_validation_logs(custodian_id, validation_logs_update_custodian_validation_logs_request)

Enable or Disable All Validation Logs for a Custodian Across Projects/Registries

Bulk update the enabled flag for all validation logs tied to a custodian and any project/registry.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_logs_update_custodian_validation_logs200_response import ValidationLogsUpdateCustodianValidationLogs200Response
from safepeopleregistry_api_sdk.models.validation_logs_update_custodian_validation_logs_request import ValidationLogsUpdateCustodianValidationLogsRequest
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
    api_instance = safepeopleregistry_api_sdk.ValidationLogsApi(api_client)
    custodian_id = 56 # int | The ID of the custodian entity
    validation_logs_update_custodian_validation_logs_request = safepeopleregistry_api_sdk.ValidationLogsUpdateCustodianValidationLogsRequest() # ValidationLogsUpdateCustodianValidationLogsRequest | 

    try:
        # Enable or Disable All Validation Logs for a Custodian Across Projects/Registries
        api_response = api_instance.validation_logs_update_custodian_validation_logs(custodian_id, validation_logs_update_custodian_validation_logs_request)
        print("The response of ValidationLogsApi->validation_logs_update_custodian_validation_logs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationLogsApi->validation_logs_update_custodian_validation_logs: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| The ID of the custodian entity | 
 **validation_logs_update_custodian_validation_logs_request** | [**ValidationLogsUpdateCustodianValidationLogsRequest**](ValidationLogsUpdateCustodianValidationLogsRequest.md)|  | 

### Return type

[**ValidationLogsUpdateCustodianValidationLogs200Response**](ValidationLogsUpdateCustodianValidationLogs200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Validation logs updated successfully |  -  |
**400** | Invalid request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

