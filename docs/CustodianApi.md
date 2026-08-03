# safepeopleregistry_api_sdk.CustodianApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**custodian_add_project**](CustodianApi.md#custodian_add_project) | **POST** /api/v1/custodians/{custodianId}/projects | Custodian@addProject
[**custodian_destroy**](CustodianApi.md#custodian_destroy) | **DELETE** /api/v1/custodians/{id} | Custodian@destroy
[**custodian_get_organisations**](CustodianApi.md#custodian_get_organisations) | **GET** /api/v1/custodian/{custodianId}/organisations | Return all custodian organisations with projects
[**custodian_get_projects**](CustodianApi.md#custodian_get_projects) | **GET** /api/v1/custodian/{custodianId}/projects | Return all projects associated with a custodian
[**custodian_get_projects_users**](CustodianApi.md#custodian_get_projects_users) | **GET** /api/v1/custodians/{custodianId}/projects_users | Get all users associated with custodian&#39;s projects
[**custodian_get_user_projects**](CustodianApi.md#custodian_get_user_projects) | **GET** /api/v1/custodian/{custodianId}/users/{userId}/projects | Return all custodian projects associated with a user
[**custodian_index**](CustodianApi.md#custodian_index) | **GET** /api/v1/custodians | Custodian@index
[**custodian_show**](CustodianApi.md#custodian_show) | **GET** /api/v1/custodians/{id} | Custodian@show
[**custodian_show_by_unique_identifier**](CustodianApi.md#custodian_show_by_unique_identifier) | **GET** /api/v1/custodians/identifier/{id} | Custodian@showByUniqueIdentifier
[**custodian_store**](CustodianApi.md#custodian_store) | **POST** /api/v1/custodians | Custodian@store
[**custodian_update**](CustodianApi.md#custodian_update) | **PUT** /api/v1/custodians/{id} | Custodian@update


# **custodian_add_project**
> CustodianAddProject201Response custodian_add_project(custodian_id, custodian_add_project_request)

Custodian@addProject

Create a project for a custodian

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_add_project201_response import CustodianAddProject201Response
from safepeopleregistry_api_sdk.models.custodian_add_project_request import CustodianAddProjectRequest
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
    api_instance = safepeopleregistry_api_sdk.CustodianApi(api_client)
    custodian_id = 56 # int | ID of the custodian
    custodian_add_project_request = safepeopleregistry_api_sdk.CustodianAddProjectRequest() # CustodianAddProjectRequest | Project definition

    try:
        # Custodian@addProject
        api_response = api_instance.custodian_add_project(custodian_id, custodian_add_project_request)
        print("The response of CustodianApi->custodian_add_project:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianApi->custodian_add_project: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 
 **custodian_add_project_request** | [**CustodianAddProjectRequest**](CustodianAddProjectRequest.md)| Project definition | 

### Return type

[**CustodianAddProject201Response**](CustodianAddProject201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_destroy**
> AffiliationDestroy200Response custodian_destroy(id)

Custodian@destroy

Delete a Custodian entry from the system

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
    api_instance = safepeopleregistry_api_sdk.CustodianApi(api_client)
    id = 1 # int | Custodian entry ID

    try:
        # Custodian@destroy
        api_response = api_instance.custodian_destroy(id)
        print("The response of CustodianApi->custodian_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianApi->custodian_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Custodian entry ID | 

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
**400** | Invalid argument(s) |  -  |
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_get_organisations**
> CustodianGetOrganisations200Response custodian_get_organisations(custodian_id)

Return all custodian organisations with projects

Fetch a list of custodians organisations with projects, along with pagination details.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_get_organisations200_response import CustodianGetOrganisations200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianApi(api_client)
    custodian_id = 1 # int | The ID of the custodian whose organisations are to be retrieved

    try:
        # Return all custodian organisations with projects
        api_response = api_instance.custodian_get_organisations(custodian_id)
        print("The response of CustodianApi->custodian_get_organisations:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianApi->custodian_get_organisations: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| The ID of the custodian whose organisations are to be retrieved | 

### Return type

[**CustodianGetOrganisations200Response**](CustodianGetOrganisations200Response.md)

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

# **custodian_get_projects**
> CustodianGetProjects200Response custodian_get_projects(custodian_id)

Return all projects associated with a custodian

Fetch a list of projects along with pagination details for a specified custodian.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_get_projects200_response import CustodianGetProjects200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianApi(api_client)
    custodian_id = 1 # int | The ID of the custodian whose projects are to be retrieved

    try:
        # Return all projects associated with a custodian
        api_response = api_instance.custodian_get_projects(custodian_id)
        print("The response of CustodianApi->custodian_get_projects:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianApi->custodian_get_projects: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| The ID of the custodian whose projects are to be retrieved | 

### Return type

[**CustodianGetProjects200Response**](CustodianGetProjects200Response.md)

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
**404** | Custodian not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_get_projects_users**
> CustodianGetProjectsUsers200Response custodian_get_projects_users(custodian_id)

Get all users associated with custodian's projects

Returns paginated users for all projects under a specific custodian.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_get_projects_users200_response import CustodianGetProjectsUsers200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianApi(api_client)
    custodian_id = 56 # int | Custodian ID

    try:
        # Get all users associated with custodian's projects
        api_response = api_instance.custodian_get_projects_users(custodian_id)
        print("The response of CustodianApi->custodian_get_projects_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianApi->custodian_get_projects_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| Custodian ID | 

### Return type

[**CustodianGetProjectsUsers200Response**](CustodianGetProjectsUsers200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | List of users |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Custodian not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_get_user_projects**
> CustodianGetUserProjects200Response custodian_get_user_projects(custodian_id, user_id)

Return all custodian projects associated with a user

Fetch a list of custodians projects associated with a user, along with pagination details.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_get_user_projects200_response import CustodianGetUserProjects200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianApi(api_client)
    custodian_id = 1 # int | The ID of the custodian whose projects are to be retrieved
    user_id = 1 # int | The ID of the user whose projects are to be retrieved

    try:
        # Return all custodian projects associated with a user
        api_response = api_instance.custodian_get_user_projects(custodian_id, user_id)
        print("The response of CustodianApi->custodian_get_user_projects:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianApi->custodian_get_user_projects: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| The ID of the custodian whose projects are to be retrieved | 
 **user_id** | **int**| The ID of the user whose projects are to be retrieved | 

### Return type

[**CustodianGetUserProjects200Response**](CustodianGetUserProjects200Response.md)

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
**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_index**
> CustodianIndex200Response custodian_index()

Custodian@index

Return a list of Custodians

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_index200_response import CustodianIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianApi(api_client)

    try:
        # Custodian@index
        api_response = api_instance.custodian_index()
        print("The response of CustodianApi->custodian_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianApi->custodian_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CustodianIndex200Response**](CustodianIndex200Response.md)

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

# **custodian_show**
> CustodianIndex200Response custodian_show(id)

Custodian@show

Return an Custodian entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_index200_response import CustodianIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianApi(api_client)
    id = 1 # int | Custodian ID

    try:
        # Custodian@show
        api_response = api_instance.custodian_show(id)
        print("The response of CustodianApi->custodian_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianApi->custodian_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Custodian ID | 

### Return type

[**CustodianIndex200Response**](CustodianIndex200Response.md)

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

# **custodian_show_by_unique_identifier**
> CustodianIndex200Response custodian_show_by_unique_identifier(id)

Custodian@showByUniqueIdentifier

Return an Custodian entry by Unique Identifier

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_index200_response import CustodianIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianApi(api_client)
    id = 'c3eddb33-db74-4ea7-961a-778740f17e25' # str | Custodian Unique Identifier

    try:
        # Custodian@showByUniqueIdentifier
        api_response = api_instance.custodian_show_by_unique_identifier(id)
        print("The response of CustodianApi->custodian_show_by_unique_identifier:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianApi->custodian_show_by_unique_identifier: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **str**| Custodian Unique Identifier | 

### Return type

[**CustodianIndex200Response**](CustodianIndex200Response.md)

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

# **custodian_store**
> CustodianStore201Response custodian_store(custodian_store_request)

Custodian@store

Create a Custodian entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_store201_response import CustodianStore201Response
from safepeopleregistry_api_sdk.models.custodian_store_request import CustodianStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.CustodianApi(api_client)
    custodian_store_request = safepeopleregistry_api_sdk.CustodianStoreRequest() # CustodianStoreRequest | Custodian definition

    try:
        # Custodian@store
        api_response = api_instance.custodian_store(custodian_store_request)
        print("The response of CustodianApi->custodian_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianApi->custodian_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_store_request** | [**CustodianStoreRequest**](CustodianStoreRequest.md)| Custodian definition | 

### Return type

[**CustodianStore201Response**](CustodianStore201Response.md)

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

# **custodian_update**
> CustodianStore201Response custodian_update(id, custodian_store_request)

Custodian@update

Edit a Custodian entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_store201_response import CustodianStore201Response
from safepeopleregistry_api_sdk.models.custodian_store_request import CustodianStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.CustodianApi(api_client)
    id = 1 # int | Custodian ID
    custodian_store_request = safepeopleregistry_api_sdk.CustodianStoreRequest() # CustodianStoreRequest | Custodian definition

    try:
        # Custodian@update
        api_response = api_instance.custodian_update(id, custodian_store_request)
        print("The response of CustodianApi->custodian_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianApi->custodian_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Custodian ID | 
 **custodian_store_request** | [**CustodianStoreRequest**](CustodianStoreRequest.md)| Custodian definition | 

### Return type

[**CustodianStore201Response**](CustodianStore201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Invalid argument(s) |  -  |
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

