# safepeopleregistry_api_sdk.OrganisationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**organisation_get_delegates**](OrganisationApi.md#organisation_get_delegates) | **GET** /api/v1/organisations/{id}/delegates | Return all delegates associated with an organisation
[**organisation_get_projects**](OrganisationApi.md#organisation_get_projects) | **GET** /api/v1/organisations/{id}/projects | organisation@getProjects
[**organisation_get_sponsorships_projects**](OrganisationApi.md#organisation_get_sponsorships_projects) | **GET** /api/v1/organisations/{id}/projects/sponsorships | organisation@getSponsorshipsProjects
[**organisation_get_users**](OrganisationApi.md#organisation_get_users) | **GET** /api/v1/organisations/{id}/users | organisation@getUsers
[**organisation_index**](OrganisationApi.md#organisation_index) | **GET** /api/v1/organisations | organisation@index


# **organisation_get_delegates**
> OrganisationGetDelegates200Response organisation_get_delegates(id)

Return all delegates associated with an organisation

Return all delegates associated with an organisation

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisation_get_delegates200_response import OrganisationGetDelegates200Response
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
    api_instance = safepeopleregistry_api_sdk.OrganisationApi(api_client)
    id = 1 # int | Organisation ID

    try:
        # Return all delegates associated with an organisation
        api_response = api_instance.organisation_get_delegates(id)
        print("The response of OrganisationApi->organisation_get_delegates:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationApi->organisation_get_delegates: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Organisation ID | 

### Return type

[**OrganisationGetDelegates200Response**](OrganisationGetDelegates200Response.md)

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

# **organisation_get_projects**
> OrganisationGetProjects200Response organisation_get_projects(id)

organisation@getProjects

Return an all projects associated with an organisation (i.e. data-custodian)

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisation_get_projects200_response import OrganisationGetProjects200Response
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
    api_instance = safepeopleregistry_api_sdk.OrganisationApi(api_client)
    id = 1 # int | Organisation ID

    try:
        # organisation@getProjects
        api_response = api_instance.organisation_get_projects(id)
        print("The response of OrganisationApi->organisation_get_projects:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationApi->organisation_get_projects: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Organisation ID | 

### Return type

[**OrganisationGetProjects200Response**](OrganisationGetProjects200Response.md)

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

# **organisation_get_sponsorships_projects**
> OrganisationGetProjects200Response organisation_get_sponsorships_projects(id)

organisation@getSponsorshipsProjects

Return an all projects associated with an organisation with sponsorships (i.e. data-custodian)

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisation_get_projects200_response import OrganisationGetProjects200Response
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
    api_instance = safepeopleregistry_api_sdk.OrganisationApi(api_client)
    id = 1 # int | Organisation ID

    try:
        # organisation@getSponsorshipsProjects
        api_response = api_instance.organisation_get_sponsorships_projects(id)
        print("The response of OrganisationApi->organisation_get_sponsorships_projects:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationApi->organisation_get_sponsorships_projects: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Organisation ID | 

### Return type

[**OrganisationGetProjects200Response**](OrganisationGetProjects200Response.md)

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

# **organisation_get_users**
> OrganisationGetUsers200Response organisation_get_users(id)

organisation@getUsers

Return all users associated with an organisation

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisation_get_users200_response import OrganisationGetUsers200Response
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
    api_instance = safepeopleregistry_api_sdk.OrganisationApi(api_client)
    id = 1 # int | Organisation ID

    try:
        # organisation@getUsers
        api_response = api_instance.organisation_get_users(id)
        print("The response of OrganisationApi->organisation_get_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationApi->organisation_get_users: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Organisation ID | 

### Return type

[**OrganisationGetUsers200Response**](OrganisationGetUsers200Response.md)

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

# **organisation_index**
> OrganisationIndex200Response organisation_index()

organisation@index

Return a list of organisations

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.organisation_index200_response import OrganisationIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.OrganisationApi(api_client)

    try:
        # organisation@index
        api_response = api_instance.organisation_index()
        print("The response of OrganisationApi->organisation_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OrganisationApi->organisation_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**OrganisationIndex200Response**](OrganisationIndex200Response.md)

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

