# safepeopleregistry_api_sdk.ProjectDetailsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**project_details_destroy**](ProjectDetailsApi.md#project_details_destroy) | **DELETE** /api/v1/project_details/{id} | ProjectDetails@destroy
[**project_details_store**](ProjectDetailsApi.md#project_details_store) | **POST** /api/v1/project_details | ProjectDetails@store
[**project_details_update**](ProjectDetailsApi.md#project_details_update) | **PUT** /api/v1/project_details/{id} | ProjectDetails@update


# **project_details_destroy**
> AffiliationDestroy200Response project_details_destroy(id)

ProjectDetails@destroy

Delete a ProjectDetail entry from the system

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.affiliation_destroy200_response import AffiliationDestroy200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectDetailsApi(api_client)
    id = 1 # int | ProjectDetails entry ID

    try:
        # ProjectDetails@destroy
        api_response = api_instance.project_details_destroy(id)
        print("The response of ProjectDetailsApi->project_details_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectDetailsApi->project_details_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ProjectDetails entry ID | 

### Return type

[**AffiliationDestroy200Response**](AffiliationDestroy200Response.md)

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
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **project_details_store**
> IdentityStore201Response project_details_store(project_detail)

ProjectDetails@store

Create a ProjectDetail

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.identity_store201_response import IdentityStore201Response
from safepeopleregistry_api_sdk.models.project_detail import ProjectDetail
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
    api_instance = safepeopleregistry_api_sdk.ProjectDetailsApi(api_client)
    project_detail = safepeopleregistry_api_sdk.ProjectDetail() # ProjectDetail | ProjectDetail definition

    try:
        # ProjectDetails@store
        api_response = api_instance.project_details_store(project_detail)
        print("The response of ProjectDetailsApi->project_details_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectDetailsApi->project_details_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_detail** | [**ProjectDetail**](ProjectDetail.md)| ProjectDetail definition | 

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
**404** | Not found response |  -  |
**201** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **project_details_update**
> ProjectDetailsUpdate200Response project_details_update(id, project_detail)

ProjectDetails@update

Update a ProjectDetail entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_detail import ProjectDetail
from safepeopleregistry_api_sdk.models.project_details_update200_response import ProjectDetailsUpdate200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectDetailsApi(api_client)
    id = 1 # int | ProjectDetails entry ID
    project_detail = safepeopleregistry_api_sdk.ProjectDetail() # ProjectDetail | ProjectDetails definition

    try:
        # ProjectDetails@update
        api_response = api_instance.project_details_update(id, project_detail)
        print("The response of ProjectDetailsApi->project_details_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectDetailsApi->project_details_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ProjectDetails entry ID | 
 **project_detail** | [**ProjectDetail**](ProjectDetail.md)| ProjectDetails definition | 

### Return type

[**ProjectDetailsUpdate200Response**](ProjectDetailsUpdate200Response.md)

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

