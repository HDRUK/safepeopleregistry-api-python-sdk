# safepeopleregistry_api_sdk.CustodianUsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**custodian_users_index**](CustodianUsersApi.md#custodian_users_index) | **GET** /api/v1/custodian_users | Return a list of Custodian Users


# **custodian_users_index**
> CustodianUsersIndex200Response custodian_users_index()

Return a list of Custodian Users

Return a list of Custodian Users

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_users_index200_response import CustodianUsersIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianUsersApi(api_client)

    try:
        # Return a list of Custodian Users
        api_response = api_instance.custodian_users_index()
        print("The response of CustodianUsersApi->custodian_users_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianUsersApi->custodian_users_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**CustodianUsersIndex200Response**](CustodianUsersIndex200Response.md)

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

