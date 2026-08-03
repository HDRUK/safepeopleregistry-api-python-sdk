# safepeopleregistry_api_sdk.AffiliationApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**affiliation_destroy**](AffiliationApi.md#affiliation_destroy) | **DELETE** /api/v1/training/{id} | Affiliation@destroy


# **affiliation_destroy**
> AffiliationDestroy200Response affiliation_destroy(id)

Affiliation@destroy

Delete a affiliation entry from the system

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
    api_instance = safepeopleregistry_api_sdk.AffiliationApi(api_client)
    id = 1 # int | Affiliation entry ID

    try:
        # Affiliation@destroy
        api_response = api_instance.affiliation_destroy(id)
        print("The response of AffiliationApi->affiliation_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AffiliationApi->affiliation_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Affiliation entry ID | 

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

