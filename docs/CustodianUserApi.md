# safepeopleregistry_api_sdk.CustodianUserApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**custodian_user_bulk_store**](CustodianUserApi.md#custodian_user_bulk_store) | **POST** /api/v1/custodian_users/bulk | Create multiple CustodianUser entries


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

