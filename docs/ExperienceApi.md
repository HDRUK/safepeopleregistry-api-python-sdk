# safepeopleregistry_api_sdk.ExperienceApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**experience_destroy**](ExperienceApi.md#experience_destroy) | **DELETE** /api/v1/experiences/{id} | Experience@destroy
[**experience_index**](ExperienceApi.md#experience_index) | **GET** /api/v1/experiences | Experience@index
[**experience_show**](ExperienceApi.md#experience_show) | **GET** /api/v1/experiences/{id} | Experience@show
[**experience_store**](ExperienceApi.md#experience_store) | **POST** /api/v1/experiences | Experience@store
[**experience_update**](ExperienceApi.md#experience_update) | **PUT** /api/v1/experiences/{id} | Experience@update


# **experience_destroy**
> AffiliationDestroy200Response experience_destroy(id)

Experience@destroy

Delete a Experience entry from the system

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
    api_instance = safepeopleregistry_api_sdk.ExperienceApi(api_client)
    id = 1 # int | Experience entry ID

    try:
        # Experience@destroy
        api_response = api_instance.experience_destroy(id)
        print("The response of ExperienceApi->experience_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExperienceApi->experience_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Experience entry ID | 

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

# **experience_index**
> ExperienceIndex200Response experience_index()

Experience@index

Return a list of Experience entries

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.experience_index200_response import ExperienceIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.ExperienceApi(api_client)

    try:
        # Experience@index
        api_response = api_instance.experience_index()
        print("The response of ExperienceApi->experience_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExperienceApi->experience_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ExperienceIndex200Response**](ExperienceIndex200Response.md)

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

# **experience_show**
> ExperienceShow200Response experience_show(id)

Experience@show

Return an Experience entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.experience_show200_response import ExperienceShow200Response
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
    api_instance = safepeopleregistry_api_sdk.ExperienceApi(api_client)
    id = 1 # int | Experience entry ID

    try:
        # Experience@show
        api_response = api_instance.experience_show(id)
        print("The response of ExperienceApi->experience_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExperienceApi->experience_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Experience entry ID | 

### Return type

[**ExperienceShow200Response**](ExperienceShow200Response.md)

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

# **experience_store**
> ExperienceStore201Response experience_store(experience_store_request)

Experience@store

Create an Experience entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.experience_store201_response import ExperienceStore201Response
from safepeopleregistry_api_sdk.models.experience_store_request import ExperienceStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.ExperienceApi(api_client)
    experience_store_request = safepeopleregistry_api_sdk.ExperienceStoreRequest() # ExperienceStoreRequest | Experience definition

    try:
        # Experience@store
        api_response = api_instance.experience_store(experience_store_request)
        print("The response of ExperienceApi->experience_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExperienceApi->experience_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **experience_store_request** | [**ExperienceStoreRequest**](ExperienceStoreRequest.md)| Experience definition | 

### Return type

[**ExperienceStore201Response**](ExperienceStore201Response.md)

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

# **experience_update**
> ExperienceUpdate200Response experience_update(id, experience_store_request)

Experience@update

Update an Experience entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.experience_store_request import ExperienceStoreRequest
from safepeopleregistry_api_sdk.models.experience_update200_response import ExperienceUpdate200Response
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
    api_instance = safepeopleregistry_api_sdk.ExperienceApi(api_client)
    id = 1 # int | Experience entry ID
    experience_store_request = safepeopleregistry_api_sdk.ExperienceStoreRequest() # ExperienceStoreRequest | Experience definition

    try:
        # Experience@update
        api_response = api_instance.experience_update(id, experience_store_request)
        print("The response of ExperienceApi->experience_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExperienceApi->experience_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Experience entry ID | 
 **experience_store_request** | [**ExperienceStoreRequest**](ExperienceStoreRequest.md)| Experience definition | 

### Return type

[**ExperienceUpdate200Response**](ExperienceUpdate200Response.md)

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

