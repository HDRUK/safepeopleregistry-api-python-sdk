# safepeopleregistry_api_sdk.ProjectRoleApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**project_role_index**](ProjectRoleApi.md#project_role_index) | **GET** /api/v1/project_roles | ProjectRole@index
[**project_role_show**](ProjectRoleApi.md#project_role_show) | **GET** /api/v1/project_roles/{id} | ProjectRole@show
[**project_role_store**](ProjectRoleApi.md#project_role_store) | **POST** /api/v1/project_roles | ProjectRole@store
[**project_role_update**](ProjectRoleApi.md#project_role_update) | **PUT** /api/v1/project_roles/{id} | ProjectRole@update


# **project_role_index**
> ProjectRoleIndex200Response project_role_index()

ProjectRole@index

Return a list of ProjectRole

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_role_index200_response import ProjectRoleIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectRoleApi(api_client)

    try:
        # ProjectRole@index
        api_response = api_instance.project_role_index()
        print("The response of ProjectRoleApi->project_role_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectRoleApi->project_role_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ProjectRoleIndex200Response**](ProjectRoleIndex200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **project_role_show**
> ProjectRoleIndex200Response project_role_show(id)

ProjectRole@show

Return a ProjectRole

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_role_index200_response import ProjectRoleIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectRoleApi(api_client)
    id = 1 # int | ProjectRole entry ID

    try:
        # ProjectRole@show
        api_response = api_instance.project_role_show(id)
        print("The response of ProjectRoleApi->project_role_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectRoleApi->project_role_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ProjectRole entry ID | 

### Return type

[**ProjectRoleIndex200Response**](ProjectRoleIndex200Response.md)

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

# **project_role_store**
> IdentityStore201Response project_role_store(project_role)

ProjectRole@store

Create a ProjectRole

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.identity_store201_response import IdentityStore201Response
from safepeopleregistry_api_sdk.models.project_role import ProjectRole
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
    api_instance = safepeopleregistry_api_sdk.ProjectRoleApi(api_client)
    project_role = safepeopleregistry_api_sdk.ProjectRole() # ProjectRole | ProjectRole definition

    try:
        # ProjectRole@store
        api_response = api_instance.project_role_store(project_role)
        print("The response of ProjectRoleApi->project_role_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectRoleApi->project_role_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_role** | [**ProjectRole**](ProjectRole.md)| ProjectRole definition | 

### Return type

[**IdentityStore201Response**](IdentityStore201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Success |  -  |
**404** | Not found response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **project_role_update**
> ProjectRoleUpdate200Response project_role_update(id, project_role)

ProjectRole@update

Update a ProjectRole entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_role import ProjectRole
from safepeopleregistry_api_sdk.models.project_role_update200_response import ProjectRoleUpdate200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectRoleApi(api_client)
    id = 1 # int | ProjectRole entry ID
    project_role = safepeopleregistry_api_sdk.ProjectRole() # ProjectRole | ProjectRole definition

    try:
        # ProjectRole@update
        api_response = api_instance.project_role_update(id, project_role)
        print("The response of ProjectRoleApi->project_role_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectRoleApi->project_role_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ProjectRole entry ID | 
 **project_role** | [**ProjectRole**](ProjectRole.md)| ProjectRole definition | 

### Return type

[**ProjectRoleUpdate200Response**](ProjectRoleUpdate200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Not found response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

