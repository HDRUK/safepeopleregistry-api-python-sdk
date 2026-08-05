# safepeopleregistry_api_sdk.VendorWebhookReceiverApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**vendor_webhook_receiver_receive**](VendorWebhookReceiverApi.md#vendor_webhook_receiver_receive) | **POST** /api/v1/webhooks/{provider} | Receive a webhook callback from a vendor


# **vendor_webhook_receiver_receive**
> VendorWebhookReceiverReceive200Response vendor_webhook_receiver_receive(provider, body)

Receive a webhook callback from a vendor

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.vendor_webhook_receiver_receive200_response import VendorWebhookReceiverReceive200Response
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
    api_instance = safepeopleregistry_api_sdk.VendorWebhookReceiverApi(api_client)
    provider = 'example-provider' # str | Name of the vendor providing the webhook
    body = {"event":"user.created","data":{"id":123,"name":"John Doe"}} # object | 

    try:
        # Receive a webhook callback from a vendor
        api_response = api_instance.vendor_webhook_receiver_receive(provider, body)
        print("The response of VendorWebhookReceiverApi->vendor_webhook_receiver_receive:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling VendorWebhookReceiverApi->vendor_webhook_receiver_receive: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **provider** | **str**| Name of the vendor providing the webhook | 
 **body** | **object**|  | 

### Return type

[**VendorWebhookReceiverReceive200Response**](VendorWebhookReceiverReceive200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Webhook processed successfully |  -  |
**400** | Invalid argument(s) |  -  |
**500** | Internal server error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

