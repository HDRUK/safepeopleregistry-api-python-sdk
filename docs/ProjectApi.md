# safepeopleregistry_api_sdk.ProjectApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**project_destroy**](ProjectApi.md#project_destroy) | **DELETE** /api/v1/projects/{id} | Project@destroy
[**project_get_all_users_flag_project_by_user_id**](ProjectApi.md#project_get_all_users_flag_project_by_user_id) | **GET** /api/v1/projects/{projectId}/all_users/{userId} | Get all users by projectID and userID
[**project_get_project_by_id_and_organisation_id**](ProjectApi.md#project_get_project_by_id_and_organisation_id) | **GET** /api/v1/projects/{projectId}/organisations/{organisationId} | Get project details by projectID and organisationID
[**project_get_project_by_id_and_user_id**](ProjectApi.md#project_get_project_by_id_and_user_id) | **GET** /api/v1/projects/{projectId}/users/{userId} | Get project details by projectID and userID
[**project_get_project_users**](ProjectApi.md#project_get_project_users) | **GET** /api/v1/projects/{id}/users | Project@getProjectUsers
[**project_get_project_users_by_organisation_id**](ProjectApi.md#project_get_project_users_by_organisation_id) | **GET** /api/v1/projects/{projectId}/organisations/{organisationId}/users | Get all users by projectID and organisationID
[**project_index**](ProjectApi.md#project_index) | **GET** /api/v1/projects | Project@index
[**project_make_primary_contact**](ProjectApi.md#project_make_primary_contact) | **PUT** /api/v1/projects/{id}/users/{registryId}/primary_contact | Project@edit
[**project_show**](ProjectApi.md#project_show) | **GET** /api/v1/projects/{id} | Project@show
[**project_store**](ProjectApi.md#project_store) | **POST** /api/v1/projects | Project@store
[**project_update**](ProjectApi.md#project_update) | **PUT** /api/v1/projects/{id} | Project@update
[**project_update_all_project_users**](ProjectApi.md#project_update_all_project_users) | **PUT** /api/v1/projects/{id}/all_users | Project@updateAllProjectUsers


# **project_destroy**
> AffiliationDestroy200Response project_destroy(id)

Project@destroy

Delete a Project entry from the system

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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)
    id = 1 # int | Project entry ID

    try:
        # Project@destroy
        api_response = api_instance.project_destroy(id)
        print("The response of ProjectApi->project_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Project entry ID | 

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

# **project_get_all_users_flag_project_by_user_id**
> ProjectGetAllUsersFlagProjectByUserId200Response project_get_all_users_flag_project_by_user_id(user_id, project_id)

Get all users by projectID and userID

Fetches users for a project.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_get_all_users_flag_project_by_user_id200_response import ProjectGetAllUsersFlagProjectByUserId200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)
    user_id = 56 # int | ID of the user
    project_id = 56 # int | ID of the project

    try:
        # Get all users by projectID and userID
        api_response = api_instance.project_get_all_users_flag_project_by_user_id(user_id, project_id)
        print("The response of ProjectApi->project_get_all_users_flag_project_by_user_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_get_all_users_flag_project_by_user_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| ID of the user | 
 **project_id** | **int**| ID of the project | 

### Return type

[**ProjectGetAllUsersFlagProjectByUserId200Response**](ProjectGetAllUsersFlagProjectByUserId200Response.md)

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
**403** | Forbidden |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **project_get_project_by_id_and_organisation_id**
> CustodiansGetOrganisationUsers200Response project_get_project_by_id_and_organisation_id(organisation_id, project_id)

Get project details by projectID and organisationID

Fetches project given organisation and project IDs.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodians_get_organisation_users200_response import CustodiansGetOrganisationUsers200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)
    organisation_id = 56 # int | ID of the organisation
    project_id = 56 # int | ID of the project

    try:
        # Get project details by projectID and organisationID
        api_response = api_instance.project_get_project_by_id_and_organisation_id(organisation_id, project_id)
        print("The response of ProjectApi->project_get_project_by_id_and_organisation_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_get_project_by_id_and_organisation_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organisation_id** | **int**| ID of the organisation | 
 **project_id** | **int**| ID of the project | 

### Return type

[**CustodiansGetOrganisationUsers200Response**](CustodiansGetOrganisationUsers200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully retrieved project |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Project not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **project_get_project_by_id_and_user_id**
> ProjectGetProjectByIdAndUserId200Response project_get_project_by_id_and_user_id(user_id, project_id)

Get project details by projectID and userID

Fetches project given user and project IDs.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_get_project_by_id_and_user_id200_response import ProjectGetProjectByIdAndUserId200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)
    user_id = 56 # int | ID of the user
    project_id = 56 # int | ID of the project

    try:
        # Get project details by projectID and userID
        api_response = api_instance.project_get_project_by_id_and_user_id(user_id, project_id)
        print("The response of ProjectApi->project_get_project_by_id_and_user_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_get_project_by_id_and_user_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| ID of the user | 
 **project_id** | **int**| ID of the project | 

### Return type

[**ProjectGetProjectByIdAndUserId200Response**](ProjectGetProjectByIdAndUserId200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully retrieved project |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Project not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **project_get_project_users**
> ProjectGetProjectUsers200Response project_get_project_users(id)

Project@getProjectUsers

Return project users by project ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_get_project_users200_response import ProjectGetProjectUsers200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)
    id = 1 # int | Project entry ID

    try:
        # Project@getProjectUsers
        api_response = api_instance.project_get_project_users(id)
        print("The response of ProjectApi->project_get_project_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_get_project_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Project entry ID | 

### Return type

[**ProjectGetProjectUsers200Response**](ProjectGetProjectUsers200Response.md)

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

# **project_get_project_users_by_organisation_id**
> CustodiansGetOrganisationUsers200Response project_get_project_users_by_organisation_id(organisation_id, project_id)

Get all users by projectID and organisationID

Fetches users given organisation and project IDs.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodians_get_organisation_users200_response import CustodiansGetOrganisationUsers200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)
    organisation_id = 56 # int | ID of the organisation
    project_id = 56 # int | ID of the project

    try:
        # Get all users by projectID and organisationID
        api_response = api_instance.project_get_project_users_by_organisation_id(organisation_id, project_id)
        print("The response of ProjectApi->project_get_project_users_by_organisation_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_get_project_users_by_organisation_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organisation_id** | **int**| ID of the organisation | 
 **project_id** | **int**| ID of the project | 

### Return type

[**CustodiansGetOrganisationUsers200Response**](CustodiansGetOrganisationUsers200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successfully retrieved organisation users |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Organisation users not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **project_index**
> ProjectIndex200Response project_index()

Project@index

Return a list of Projects

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_index200_response import ProjectIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)

    try:
        # Project@index
        api_response = api_instance.project_index()
        print("The response of ProjectApi->project_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ProjectIndex200Response**](ProjectIndex200Response.md)

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

# **project_make_primary_contact**
> ProjectMakePrimaryContact200Response project_make_primary_contact(id, registry_id, project_make_primary_contact_request)

Project@edit

Make user a primary contact

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_make_primary_contact200_response import ProjectMakePrimaryContact200Response
from safepeopleregistry_api_sdk.models.project_make_primary_contact_request import ProjectMakePrimaryContactRequest
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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)
    id = 1 # int | Project entry ID
    registry_id = 1 # int | Registry ID
    project_make_primary_contact_request = safepeopleregistry_api_sdk.ProjectMakePrimaryContactRequest() # ProjectMakePrimaryContactRequest | Project definition

    try:
        # Project@edit
        api_response = api_instance.project_make_primary_contact(id, registry_id, project_make_primary_contact_request)
        print("The response of ProjectApi->project_make_primary_contact:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_make_primary_contact: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Project entry ID | 
 **registry_id** | **int**| Registry ID | 
 **project_make_primary_contact_request** | [**ProjectMakePrimaryContactRequest**](ProjectMakePrimaryContactRequest.md)| Project definition | 

### Return type

[**ProjectMakePrimaryContact200Response**](ProjectMakePrimaryContact200Response.md)

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

# **project_show**
> ProjectIndex200Response project_show(id)

Project@show

Return a Project entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_index200_response import ProjectIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)
    id = 1 # int | Project entry ID

    try:
        # Project@show
        api_response = api_instance.project_show(id)
        print("The response of ProjectApi->project_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Project entry ID | 

### Return type

[**ProjectIndex200Response**](ProjectIndex200Response.md)

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

# **project_store**
> AccreditationStoreByRegistryId201Response project_store(project_store_request)

Project@store

Create a Project entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.project_store_request import ProjectStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)
    project_store_request = safepeopleregistry_api_sdk.ProjectStoreRequest() # ProjectStoreRequest | Project definition

    try:
        # Project@store
        api_response = api_instance.project_store(project_store_request)
        print("The response of ProjectApi->project_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_store_request** | [**ProjectStoreRequest**](ProjectStoreRequest.md)| Project definition | 

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
**404** | Not found response |  -  |
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **project_update**
> ProjectUpdate200Response project_update(id, project_index200_response_data)

Project@update

Update a Project entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.project_index200_response_data import ProjectIndex200ResponseData
from safepeopleregistry_api_sdk.models.project_update200_response import ProjectUpdate200Response
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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)
    id = 1 # int | Project entry ID
    project_index200_response_data = safepeopleregistry_api_sdk.ProjectIndex200ResponseData() # ProjectIndex200ResponseData | Project definition

    try:
        # Project@update
        api_response = api_instance.project_update(id, project_index200_response_data)
        print("The response of ProjectApi->project_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Project entry ID | 
 **project_index200_response_data** | [**ProjectIndex200ResponseData**](ProjectIndex200ResponseData.md)| Project definition | 

### Return type

[**ProjectUpdate200Response**](ProjectUpdate200Response.md)

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

# **project_update_all_project_users**
> ONSSubmissionReceiveCSV200Response project_update_all_project_users(id, project_update_all_project_users_request)

Project@updateAllProjectUsers

Update all users associated with a project

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.ons_submission_receive_csv200_response import ONSSubmissionReceiveCSV200Response
from safepeopleregistry_api_sdk.models.project_update_all_project_users_request import ProjectUpdateAllProjectUsersRequest
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
    api_instance = safepeopleregistry_api_sdk.ProjectApi(api_client)
    id = 1 # int | Project entry ID
    project_update_all_project_users_request = safepeopleregistry_api_sdk.ProjectUpdateAllProjectUsersRequest() # ProjectUpdateAllProjectUsersRequest | Project definition

    try:
        # Project@updateAllProjectUsers
        api_response = api_instance.project_update_all_project_users(id, project_update_all_project_users_request)
        print("The response of ProjectApi->project_update_all_project_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectApi->project_update_all_project_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Project entry ID | 
 **project_update_all_project_users_request** | [**ProjectUpdateAllProjectUsersRequest**](ProjectUpdateAllProjectUsersRequest.md)| Project definition | 

### Return type

[**ONSSubmissionReceiveCSV200Response**](ONSSubmissionReceiveCSV200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success response |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Not found response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

