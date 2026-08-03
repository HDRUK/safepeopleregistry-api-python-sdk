# safepeopleregistry_api_sdk.UserApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**user_destroy**](UserApi.md#user_destroy) | **DELETE** /api/v1/users/{id} | User@destroy
[**user_index**](UserApi.md#user_index) | **GET** /api/v1/users | User@index
[**user_show**](UserApi.md#user_show) | **GET** /api/v1/users/{id} | User@show
[**user_update**](UserApi.md#user_update) | **PUT** /api/v1/users/{id} | User@update


# **user_destroy**
> AffiliationDestroy200Response user_destroy(id)

User@destroy

Delete a User entry from the system

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
    api_instance = safepeopleregistry_api_sdk.UserApi(api_client)
    id = 1 # int | User entry ID

    try:
        # User@destroy
        api_response = api_instance.user_destroy(id)
        print("The response of UserApi->user_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->user_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| User entry ID | 

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
**404** | Not found response |  -  |
**200** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **user_index**
> UserIndex200Response user_index()

User@index

Return a list of Users

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.user_index200_response import UserIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.UserApi(api_client)

    try:
        # User@index
        api_response = api_instance.user_index()
        print("The response of UserApi->user_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->user_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**UserIndex200Response**](UserIndex200Response.md)

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

# **user_show**
> UserShow200Response user_show(id)

User@show

Return a User entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.user_show200_response import UserShow200Response
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
    api_instance = safepeopleregistry_api_sdk.UserApi(api_client)
    id = 1 # int | User ID

    try:
        # User@show
        api_response = api_instance.user_show(id)
        print("The response of UserApi->user_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->user_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| User ID | 

### Return type

[**UserShow200Response**](UserShow200Response.md)

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

# **user_update**
> UserUpdate200Response user_update(id, user_update_request)

User@update

Edit a User entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.user_update200_response import UserUpdate200Response
from safepeopleregistry_api_sdk.models.user_update_request import UserUpdateRequest
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
    api_instance = safepeopleregistry_api_sdk.UserApi(api_client)
    id = 1 # int | User ID
    user_update_request = safepeopleregistry_api_sdk.UserUpdateRequest() # UserUpdateRequest | User definition

    try:
        # User@update
        api_response = api_instance.user_update(id, user_update_request)
        print("The response of UserApi->user_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->user_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| User ID | 
 **user_update_request** | [**UserUpdateRequest**](UserUpdateRequest.md)| User definition | 

### Return type

[**UserUpdate200Response**](UserUpdate200Response.md)

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
**400** | Invalid argument(s) |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

