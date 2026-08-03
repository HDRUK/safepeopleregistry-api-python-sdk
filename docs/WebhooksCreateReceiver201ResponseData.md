# WebhooksCreateReceiver201ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**custodian_id** | **int** |  | [optional] 
**url** | **str** |  | [optional] 
**webhook_event** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.webhooks_create_receiver201_response_data import WebhooksCreateReceiver201ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of WebhooksCreateReceiver201ResponseData from a JSON string
webhooks_create_receiver201_response_data_instance = WebhooksCreateReceiver201ResponseData.from_json(json)
# print the JSON string representation of the object
print(WebhooksCreateReceiver201ResponseData.to_json())

# convert the object into a dict
webhooks_create_receiver201_response_data_dict = webhooks_create_receiver201_response_data_instance.to_dict()
# create an instance of WebhooksCreateReceiver201ResponseData from a dict
webhooks_create_receiver201_response_data_from_dict = WebhooksCreateReceiver201ResponseData.from_dict(webhooks_create_receiver201_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


