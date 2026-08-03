# safepeopleregistry_api_sdk.PendingInvitesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**pending_invites_index**](PendingInvitesApi.md#pending_invites_index) | **GET** /api/v1/pending_invites | PendingInvite@index


# **pending_invites_index**
> PendingInvitesIndex200Response pending_invites_index()

PendingInvite@index

Return a list of pending invites

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.pending_invites_index200_response import PendingInvitesIndex200Response
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
    api_instance = safepeopleregistry_api_sdk.PendingInvitesApi(api_client)

    try:
        # PendingInvite@index
        api_response = api_instance.pending_invites_index()
        print("The response of PendingInvitesApi->pending_invites_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PendingInvitesApi->pending_invites_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**PendingInvitesIndex200Response**](PendingInvitesIndex200Response.md)

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

