# VendorWebhookReceiverReceive200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | **List[object]** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.vendor_webhook_receiver_receive200_response import VendorWebhookReceiverReceive200Response

# TODO update the JSON string below
json = "{}"
# create an instance of VendorWebhookReceiverReceive200Response from a JSON string
vendor_webhook_receiver_receive200_response_instance = VendorWebhookReceiverReceive200Response.from_json(json)
# print the JSON string representation of the object
print(VendorWebhookReceiverReceive200Response.to_json())

# convert the object into a dict
vendor_webhook_receiver_receive200_response_dict = vendor_webhook_receiver_receive200_response_instance.to_dict()
# create an instance of VendorWebhookReceiverReceive200Response from a dict
vendor_webhook_receiver_receive200_response_from_dict = VendorWebhookReceiverReceive200Response.from_dict(vendor_webhook_receiver_receive200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


