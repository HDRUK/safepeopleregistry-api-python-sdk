# WebhooksCreateReceiver201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**WebhooksCreateReceiver201ResponseData**](WebhooksCreateReceiver201ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.webhooks_create_receiver201_response import WebhooksCreateReceiver201Response

# TODO update the JSON string below
json = "{}"
# create an instance of WebhooksCreateReceiver201Response from a JSON string
webhooks_create_receiver201_response_instance = WebhooksCreateReceiver201Response.from_json(json)
# print the JSON string representation of the object
print(WebhooksCreateReceiver201Response.to_json())

# convert the object into a dict
webhooks_create_receiver201_response_dict = webhooks_create_receiver201_response_instance.to_dict()
# create an instance of WebhooksCreateReceiver201Response from a dict
webhooks_create_receiver201_response_from_dict = WebhooksCreateReceiver201Response.from_dict(webhooks_create_receiver201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


