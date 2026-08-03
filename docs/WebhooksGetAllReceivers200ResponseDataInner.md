# WebhooksGetAllReceivers200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**custodian_id** | **int** |  | [optional] 
**url** | **str** |  | [optional] 
**webhook_event** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**event_trigger** | [**WebhooksGetAllReceivers200ResponseDataInnerEventTrigger**](WebhooksGetAllReceivers200ResponseDataInnerEventTrigger.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.webhooks_get_all_receivers200_response_data_inner import WebhooksGetAllReceivers200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of WebhooksGetAllReceivers200ResponseDataInner from a JSON string
webhooks_get_all_receivers200_response_data_inner_instance = WebhooksGetAllReceivers200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(WebhooksGetAllReceivers200ResponseDataInner.to_json())

# convert the object into a dict
webhooks_get_all_receivers200_response_data_inner_dict = webhooks_get_all_receivers200_response_data_inner_instance.to_dict()
# create an instance of WebhooksGetAllReceivers200ResponseDataInner from a dict
webhooks_get_all_receivers200_response_data_inner_from_dict = WebhooksGetAllReceivers200ResponseDataInner.from_dict(webhooks_get_all_receivers200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


