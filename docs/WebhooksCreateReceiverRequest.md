# WebhooksCreateReceiverRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**custodian_id** | **int** |  | [optional] 
**url** | **str** |  | [optional] 
**webhook_event_id** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.webhooks_create_receiver_request import WebhooksCreateReceiverRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WebhooksCreateReceiverRequest from a JSON string
webhooks_create_receiver_request_instance = WebhooksCreateReceiverRequest.from_json(json)
# print the JSON string representation of the object
print(WebhooksCreateReceiverRequest.to_json())

# convert the object into a dict
webhooks_create_receiver_request_dict = webhooks_create_receiver_request_instance.to_dict()
# create an instance of WebhooksCreateReceiverRequest from a dict
webhooks_create_receiver_request_from_dict = WebhooksCreateReceiverRequest.from_dict(webhooks_create_receiver_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


