# safepeopleregistry_api_sdk.UsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**users_store**](UsersApi.md#users_store) | **POST** /api/v1/users | Users@store


# **users_store**
> UsersStore201Response users_store(users_store_request)

Users@store

Create a User entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.users_store201_response import UsersStore201Response
from safepeopleregistry_api_sdk.models.users_store_request import UsersStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.UsersApi(api_client)
    users_store_request = safepeopleregistry_api_sdk.UsersStoreRequest() # UsersStoreRequest | User definition

    try:
        # Users@store
        api_response = api_instance.users_store(users_store_request)
        print("The response of UsersApi->users_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->users_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **users_store_request** | [**UsersStoreRequest**](UsersStoreRequest.md)| User definition | 

### Return type

[**UsersStore201Response**](UsersStore201Response.md)

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

