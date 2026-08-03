# WebhookEventTrigger

Model representing webhook event triggers

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the webhook event trigger | [optional] 
**name** | **str** | Name of the webhook event trigger | [optional] 
**description** | **str** | Description of the webhook event trigger | [optional] 
**enabled** | **bool** | Indicates whether the webhook event trigger is enabled | [optional] 
**created_at** | **datetime** | Timestamp when the webhook event trigger was created | [optional] 
**updated_at** | **datetime** | Timestamp when the webhook event trigger was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.webhook_event_trigger import WebhookEventTrigger

# TODO update the JSON string below
json = "{}"
# create an instance of WebhookEventTrigger from a JSON string
webhook_event_trigger_instance = WebhookEventTrigger.from_json(json)
# print the JSON string representation of the object
print(WebhookEventTrigger.to_json())

# convert the object into a dict
webhook_event_trigger_dict = webhook_event_trigger_instance.to_dict()
# create an instance of WebhookEventTrigger from a dict
webhook_event_trigger_from_dict = WebhookEventTrigger.from_dict(webhook_event_trigger_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


