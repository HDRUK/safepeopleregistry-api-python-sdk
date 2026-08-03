# safepeopleregistry_api_sdk.DepartmentApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**department_destroy**](DepartmentApi.md#department_destroy) | **DELETE** /api/v1/departments/{id} | Delete a department
[**department_index**](DepartmentApi.md#department_index) | **GET** /api/v1/departments | Get a list of departments
[**department_show**](DepartmentApi.md#department_show) | **GET** /api/v1/departments/{id} | Get a specific department by ID
[**department_store**](DepartmentApi.md#department_store) | **POST** /api/v1/departments | Create a new department
[**department_update**](DepartmentApi.md#department_update) | **PUT** /api/v1/departments/{id} | Update an existing department


# **department_destroy**
> AffiliationDestroy200Response department_destroy(id)

Delete a department

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
    api_instance = safepeopleregistry_api_sdk.DepartmentApi(api_client)
    id = 1 # int | ID of the department

    try:
        # Delete a department
        api_response = api_instance.department_destroy(id)
        print("The response of DepartmentApi->department_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DepartmentApi->department_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the department | 

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
**200** | Deleted |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Department not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **department_index**
> List[Department] department_index()

Get a list of departments

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.department import Department
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
    api_instance = safepeopleregistry_api_sdk.DepartmentApi(api_client)

    try:
        # Get a list of departments
        api_response = api_instance.department_index()
        print("The response of DepartmentApi->department_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DepartmentApi->department_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[Department]**](Department.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **department_show**
> Department department_show(id)

Get a specific department by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.department import Department
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
    api_instance = safepeopleregistry_api_sdk.DepartmentApi(api_client)
    id = 1 # int | ID of the department

    try:
        # Get a specific department by ID
        api_response = api_instance.department_show(id)
        print("The response of DepartmentApi->department_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DepartmentApi->department_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the department | 

### Return type

[**Department**](Department.md)

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
**404** | Department not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **department_store**
> AccreditationStoreByRegistryId201Response department_store(department)

Create a new department

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.department import Department
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
    api_instance = safepeopleregistry_api_sdk.DepartmentApi(api_client)
    department = safepeopleregistry_api_sdk.Department() # Department | 

    try:
        # Create a new department
        api_response = api_instance.department_store(department)
        print("The response of DepartmentApi->department_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DepartmentApi->department_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **department** | [**Department**](Department.md)|  | 

### Return type

[**AccreditationStoreByRegistryId201Response**](AccreditationStoreByRegistryId201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Created |  -  |
**400** | Validation error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **department_update**
> Department department_update(id, department)

Update an existing department

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.department import Department
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
    api_instance = safepeopleregistry_api_sdk.DepartmentApi(api_client)
    id = 1 # int | ID of the department
    department = safepeopleregistry_api_sdk.Department() # Department | 

    try:
        # Update an existing department
        api_response = api_instance.department_update(id, department)
        print("The response of DepartmentApi->department_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DepartmentApi->department_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the department | 
 **department** | [**Department**](Department.md)|  | 

### Return type

[**Department**](Department.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Updated |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Department not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

