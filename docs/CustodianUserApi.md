# safepeopleregistry_api_sdk.CustodianUserApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**custodian_user_bulk_store**](CustodianUserApi.md#custodian_user_bulk_store) | **POST** /api/v1/custodian_users/bulk | Create multiple CustodianUser entries
[**custodian_user_destroy**](CustodianUserApi.md#custodian_user_destroy) | **DELETE** /api/v1/custodian_users/{id} | CustodianUser@destroy
[**custodian_user_show**](CustodianUserApi.md#custodian_user_show) | **GET** /api/v1/custodian_users/{id} | CustodianUser@show
[**custodian_user_store**](CustodianUserApi.md#custodian_user_store) | **POST** /api/v1/custodian_users | CustodianUser@store
[**custodian_user_update**](CustodianUserApi.md#custodian_user_update) | **PUT** /api/v1/custodian_users | CustodianUser@update


# **custodian_user_bulk_store**
> CustodianUserBulkStore201Response custodian_user_bulk_store(custodian_user_bulk_store_request)

Create multiple CustodianUser entries

Create multiple CustodianUser entries

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_user_bulk_store201_response import CustodianUserBulkStore201Response
from safepeopleregistry_api_sdk.models.custodian_user_bulk_store_request import CustodianUserBulkStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.CustodianUserApi(api_client)
    custodian_user_bulk_store_request = safepeopleregistry_api_sdk.CustodianUserBulkStoreRequest() # CustodianUserBulkStoreRequest | Array of CustodianUser definitions

    try:
        # Create multiple CustodianUser entries
        api_response = api_instance.custodian_user_bulk_store(custodian_user_bulk_store_request)
        print("The response of CustodianUserApi->custodian_user_bulk_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianUserApi->custodian_user_bulk_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_user_bulk_store_request** | [**CustodianUserBulkStoreRequest**](CustodianUserBulkStoreRequest.md)| Array of CustodianUser definitions | 

### Return type

[**CustodianUserBulkStore201Response**](CustodianUserBulkStore201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_user_destroy**
> AffiliationDestroy200Response custodian_user_destroy(id)

CustodianUser@destroy

Delete a CustodianUser entry from the system

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
    api_instance = safepeopleregistry_api_sdk.CustodianUserApi(api_client)
    id = 1 # int | CustodianUser entry ID

    try:
        # CustodianUser@destroy
        api_response = api_instance.custodian_user_destroy(id)
        print("The response of CustodianUserApi->custodian_user_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianUserApi->custodian_user_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| CustodianUser entry ID | 

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

# **custodian_user_show**
> CustodianUserShow200Response custodian_user_show(id)

CustodianUser@show

Return a CustodianUser entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_user_show200_response import CustodianUserShow200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianUserApi(api_client)
    id = 1 # int | CustodianUser entry ID

    try:
        # CustodianUser@show
        api_response = api_instance.custodian_user_show(id)
        print("The response of CustodianUserApi->custodian_user_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianUserApi->custodian_user_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| CustodianUser entry ID | 

### Return type

[**CustodianUserShow200Response**](CustodianUserShow200Response.md)

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

# **custodian_user_store**
> AccreditationStoreByRegistryId201Response custodian_user_store(custodian_user)

CustodianUser@store

Create a CustodianUser entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.custodian_user import CustodianUser
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
    api_instance = safepeopleregistry_api_sdk.CustodianUserApi(api_client)
    custodian_user = safepeopleregistry_api_sdk.CustodianUser() # CustodianUser | CustodianUser definition

    try:
        # CustodianUser@store
        api_response = api_instance.custodian_user_store(custodian_user)
        print("The response of CustodianUserApi->custodian_user_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianUserApi->custodian_user_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_user** | [**CustodianUser**](CustodianUser.md)| CustodianUser definition | 

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
**201** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_user_update**
> CustodianUserUpdate201Response custodian_user_update(custodian_user)

CustodianUser@update

Update a CustodianUser entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_user import CustodianUser
from safepeopleregistry_api_sdk.models.custodian_user_update201_response import CustodianUserUpdate201Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianUserApi(api_client)
    custodian_user = safepeopleregistry_api_sdk.CustodianUser() # CustodianUser | CustodianUser definition

    try:
        # CustodianUser@update
        api_response = api_instance.custodian_user_update(custodian_user)
        print("The response of CustodianUserApi->custodian_user_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianUserApi->custodian_user_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_user** | [**CustodianUser**](CustodianUser.md)| CustodianUser definition | 

### Return type

[**CustodianUserUpdate201Response**](CustodianUserUpdate201Response.md)

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
**400** | Invalid argument(s) |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

