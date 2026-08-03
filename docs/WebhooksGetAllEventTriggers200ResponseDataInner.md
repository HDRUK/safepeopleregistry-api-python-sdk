# WebhooksGetAllEventTriggers200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.webhooks_get_all_event_triggers200_response_data_inner import WebhooksGetAllEventTriggers200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of WebhooksGetAllEventTriggers200ResponseDataInner from a JSON string
webhooks_get_all_event_triggers200_response_data_inner_instance = WebhooksGetAllEventTriggers200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(WebhooksGetAllEventTriggers200ResponseDataInner.to_json())

# convert the object into a dict
webhooks_get_all_event_triggers200_response_data_inner_dict = webhooks_get_all_event_triggers200_response_data_inner_instance.to_dict()
# create an instance of WebhooksGetAllEventTriggers200ResponseDataInner from a dict
webhooks_get_all_event_triggers200_response_data_inner_from_dict = WebhooksGetAllEventTriggers200ResponseDataInner.from_dict(webhooks_get_all_event_triggers200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


