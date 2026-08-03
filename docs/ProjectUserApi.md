# safepeopleregistry_api_sdk.ProjectUserApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**project_user_show**](ProjectUserApi.md#project_user_show) | **GET** /api/v1/project_users/{id} | Get project user details


# **project_user_show**
> CustodianProjectUsersShow200Response project_user_show(id)

Get project user details

Returns details for a specific project user

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_project_users_show200_response import CustodianProjectUsersShow200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectUserApi(api_client)
    id = 56 # int | ID of the project user

    try:
        # Get project user details
        api_response = api_instance.project_user_show(id)
        print("The response of ProjectUserApi->project_user_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectUserApi->project_user_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the project user | 

### Return type

[**CustodianProjectUsersShow200Response**](CustodianProjectUsersShow200Response.md)

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

