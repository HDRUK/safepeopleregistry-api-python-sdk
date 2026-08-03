# safepeopleregistry_api_sdk.EndorsementApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**endorsement_index**](EndorsementApi.md#endorsement_index) | **GET** /api/v1/endorsements | Endorsement@index
[**endorsement_show**](EndorsementApi.md#endorsement_show) | **GET** /api/v1/endorsements/{id} | Endorsement@show


# **endorsement_index**
> EndorsementIndex200Response endorsement_index()

Endorsement@index

Return a list of Endorsements

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.endorsement_index200_response import EndorsementIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.EndorsementApi(api_client)

    try:
        # Endorsement@index
        api_response = api_instance.endorsement_index()
        print("The response of EndorsementApi->endorsement_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EndorsementApi->endorsement_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**EndorsementIndex200Response**](EndorsementIndex200Response.md)

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

# **endorsement_show**
> EndorsementIndex200Response endorsement_show(id)

Endorsement@show

Return an Endorsement entry by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.endorsement_index200_response import EndorsementIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.EndorsementApi(api_client)
    id = 1 # int | Endorsement entry ID

    try:
        # Endorsement@show
        api_response = api_instance.endorsement_show(id)
        print("The response of EndorsementApi->endorsement_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EndorsementApi->endorsement_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Endorsement entry ID | 

### Return type

[**EndorsementIndex200Response**](EndorsementIndex200Response.md)

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

