# safepeopleregistry_api_sdk.FeatureApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**feature_index**](FeatureApi.md#feature_index) | **GET** /api/v1/features | Feature@index


# **feature_index**
> FeatureIndex200Response feature_index()

Feature@index

Return a list of Feature entries

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.feature_index200_response import FeatureIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.FeatureApi(api_client)

    try:
        # Feature@index
        api_response = api_instance.feature_index()
        print("The response of FeatureApi->feature_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling FeatureApi->feature_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**FeatureIndex200Response**](FeatureIndex200Response.md)

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

