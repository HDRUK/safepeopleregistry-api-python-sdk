# safepeopleregistry_api_sdk.IdentityApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**identity_destroy**](IdentityApi.md#identity_destroy) | **DELETE** /api/v1/identities/{id} | Identity@destroy
[**identity_index**](IdentityApi.md#identity_index) | **GET** /api/v1/identities | Identity@index
[**identity_show**](IdentityApi.md#identity_show) | **GET** /api/v1/identities/{id} | Identity@show
[**identity_store**](IdentityApi.md#identity_store) | **POST** /api/v1/identities | Identity@store
[**identity_update**](IdentityApi.md#identity_update) | **PUT** /api/v1/identities/{id} | Identity@update


# **identity_destroy**
> AffiliationDestroy200Response identity_destroy(id)

Identity@destroy

Delete an Identity entry from the system

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
    api_instance = safepeopleregistry_api_sdk.IdentityApi(api_client)
    id = 1 # int | Identity entry ID

    try:
        # Identity@destroy
        api_response = api_instance.identity_destroy(id)
        print("The response of IdentityApi->identity_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IdentityApi->identity_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Identity entry ID | 

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

# **identity_index**
> IdentityIndex200Response identity_index()

Identity@index

Return a list of Identity entries

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.identity_index200_response import IdentityIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.IdentityApi(api_client)

    try:
        # Identity@index
        api_response = api_instance.identity_index()
        print("The response of IdentityApi->identity_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IdentityApi->identity_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**IdentityIndex200Response**](IdentityIndex200Response.md)

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

# **identity_show**
> IdentityIndex200Response identity_show(id)

Identity@show

Return an Identity entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.identity_index200_response import IdentityIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.IdentityApi(api_client)
    id = 1 # int | Identity ID

    try:
        # Identity@show
        api_response = api_instance.identity_show(id)
        print("The response of IdentityApi->identity_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IdentityApi->identity_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Identity ID | 

### Return type

[**IdentityIndex200Response**](IdentityIndex200Response.md)

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

# **identity_store**
> IdentityStore201Response identity_store(identity_store_request)

Identity@store

Create a Identity entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.identity_store201_response import IdentityStore201Response
from safepeopleregistry_api_sdk.models.identity_store_request import IdentityStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.IdentityApi(api_client)
    identity_store_request = safepeopleregistry_api_sdk.IdentityStoreRequest() # IdentityStoreRequest | Identity definition

    try:
        # Identity@store
        api_response = api_instance.identity_store(identity_store_request)
        print("The response of IdentityApi->identity_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IdentityApi->identity_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **identity_store_request** | [**IdentityStoreRequest**](IdentityStoreRequest.md)| Identity definition | 

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

# **identity_update**
> IdentityUpdate200Response identity_update(id, identity_store_request)

Identity@update

Update a Identity entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.identity_store_request import IdentityStoreRequest
from safepeopleregistry_api_sdk.models.identity_update200_response import IdentityUpdate200Response
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
    api_instance = safepeopleregistry_api_sdk.IdentityApi(api_client)
    id = 1 # int | Identity entry ID
    identity_store_request = safepeopleregistry_api_sdk.IdentityStoreRequest() # IdentityStoreRequest | Identity definition

    try:
        # Identity@update
        api_response = api_instance.identity_update(id, identity_store_request)
        print("The response of IdentityApi->identity_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IdentityApi->identity_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Identity entry ID | 
 **identity_store_request** | [**IdentityStoreRequest**](IdentityStoreRequest.md)| Identity definition | 

### Return type

[**IdentityUpdate200Response**](IdentityUpdate200Response.md)

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

