# safepeopleregistry_api_sdk.CustodianProjectUsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**custodian_project_users_index**](CustodianProjectUsersApi.md#custodian_project_users_index) | **GET** /api/v1/custodian_approvals/{custodianId}/projectUsers | List all project users associated with a custodian
[**custodian_project_users_show**](CustodianProjectUsersApi.md#custodian_project_users_show) | **GET** /api/v1/custodian_approvals/{custodianId}/projectUsers/{projectUserId} | Get custodian approval for a project user
[**custodian_project_users_update**](CustodianProjectUsersApi.md#custodian_project_users_update) | **PUT** /api/v1/custodian_approvals/{custodianId}/projectUsers/{projectUserId} | Update custodian approval for a project user


# **custodian_project_users_index**
> CustodianProjectUsersIndex200Response custodian_project_users_index(custodian_id)

List all project users associated with a custodian

Returns a list of all custodian project user approvals for a specific custodian

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_project_users_index200_response import CustodianProjectUsersIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianProjectUsersApi(api_client)
    custodian_id = 56 # int | ID of the custodian

    try:
        # List all project users associated with a custodian
        api_response = api_instance.custodian_project_users_index(custodian_id)
        print("The response of CustodianProjectUsersApi->custodian_project_users_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianProjectUsersApi->custodian_project_users_index: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 

### Return type

[**CustodianProjectUsersIndex200Response**](CustodianProjectUsersIndex200Response.md)

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

# **custodian_project_users_show**
> CustodianProjectUsersShow200Response custodian_project_users_show(custodian_id, project_user_id)

Get custodian approval for a project user

Returns custodian approval details for a specific project user

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
    api_instance = safepeopleregistry_api_sdk.CustodianProjectUsersApi(api_client)
    custodian_id = 56 # int | ID of the custodian
    project_user_id = 56 # int | ID of the project user

    try:
        # Get custodian approval for a project user
        api_response = api_instance.custodian_project_users_show(custodian_id, project_user_id)
        print("The response of CustodianProjectUsersApi->custodian_project_users_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianProjectUsersApi->custodian_project_users_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 
 **project_user_id** | **int**| ID of the project user | 

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

# **custodian_project_users_update**
> CustodianProjectUsersShow200Response custodian_project_users_update(custodian_id, project_user_id, custodian_project_users_update_request)

Update custodian approval for a project user

Updates approval status and/or comment for a project user

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_project_users_show200_response import CustodianProjectUsersShow200Response
from safepeopleregistry_api_sdk.models.custodian_project_users_update_request import CustodianProjectUsersUpdateRequest
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
    api_instance = safepeopleregistry_api_sdk.CustodianProjectUsersApi(api_client)
    custodian_id = 56 # int | ID of the custodian
    project_user_id = 56 # int | ID of the project user
    custodian_project_users_update_request = safepeopleregistry_api_sdk.CustodianProjectUsersUpdateRequest() # CustodianProjectUsersUpdateRequest | 

    try:
        # Update custodian approval for a project user
        api_response = api_instance.custodian_project_users_update(custodian_id, project_user_id, custodian_project_users_update_request)
        print("The response of CustodianProjectUsersApi->custodian_project_users_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianProjectUsersApi->custodian_project_users_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 
 **project_user_id** | **int**| ID of the project user | 
 **custodian_project_users_update_request** | [**CustodianProjectUsersUpdateRequest**](CustodianProjectUsersUpdateRequest.md)|  | 

### Return type

[**CustodianProjectUsersShow200Response**](CustodianProjectUsersShow200Response.md)

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

