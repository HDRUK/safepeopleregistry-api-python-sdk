# safepeopleregistry_api_sdk.EndorsementsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**endorsements_store**](EndorsementsApi.md#endorsements_store) | **POST** /api/v1/endorsements | Endorsements@store


# **endorsements_store**
> EndorsementsStore201Response endorsements_store(endorsements_store_request)

Endorsements@store

Create an Endorsements entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.endorsements_store201_response import EndorsementsStore201Response
from safepeopleregistry_api_sdk.models.endorsements_store_request import EndorsementsStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.EndorsementsApi(api_client)
    endorsements_store_request = safepeopleregistry_api_sdk.EndorsementsStoreRequest() # EndorsementsStoreRequest | Endorsements definition

    try:
        # Endorsements@store
        api_response = api_instance.endorsements_store(endorsements_store_request)
        print("The response of EndorsementsApi->endorsements_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EndorsementsApi->endorsements_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **endorsements_store_request** | [**EndorsementsStoreRequest**](EndorsementsStoreRequest.md)| Endorsements definition | 

### Return type

[**EndorsementsStore201Response**](EndorsementsStore201Response.md)

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

