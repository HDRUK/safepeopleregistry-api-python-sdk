# WebhooksDeleteReceiverRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.webhooks_delete_receiver_request import WebhooksDeleteReceiverRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WebhooksDeleteReceiverRequest from a JSON string
webhooks_delete_receiver_request_instance = WebhooksDeleteReceiverRequest.from_json(json)
# print the JSON string representation of the object
print(WebhooksDeleteReceiverRequest.to_json())

# convert the object into a dict
webhooks_delete_receiver_request_dict = webhooks_delete_receiver_request_instance.to_dict()
# create an instance of WebhooksDeleteReceiverRequest from a dict
webhooks_delete_receiver_request_from_dict = WebhooksDeleteReceiverRequest.from_dict(webhooks_delete_receiver_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


