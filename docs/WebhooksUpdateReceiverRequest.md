# WebhooksUpdateReceiverRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**url** | **str** |  | [optional] 
**webhook_event_id** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.webhooks_update_receiver_request import WebhooksUpdateReceiverRequest

# TODO update the JSON string below
json = "{}"
# create an instance of WebhooksUpdateReceiverRequest from a JSON string
webhooks_update_receiver_request_instance = WebhooksUpdateReceiverRequest.from_json(json)
# print the JSON string representation of the object
print(WebhooksUpdateReceiverRequest.to_json())

# convert the object into a dict
webhooks_update_receiver_request_dict = webhooks_update_receiver_request_instance.to_dict()
# create an instance of WebhooksUpdateReceiverRequest from a dict
webhooks_update_receiver_request_from_dict = WebhooksUpdateReceiverRequest.from_dict(webhooks_update_receiver_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


