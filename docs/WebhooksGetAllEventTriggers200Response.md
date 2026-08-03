# WebhooksGetAllEventTriggers200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[WebhooksGetAllEventTriggers200ResponseDataInner]**](WebhooksGetAllEventTriggers200ResponseDataInner.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.webhooks_get_all_event_triggers200_response import WebhooksGetAllEventTriggers200Response

# TODO update the JSON string below
json = "{}"
# create an instance of WebhooksGetAllEventTriggers200Response from a JSON string
webhooks_get_all_event_triggers200_response_instance = WebhooksGetAllEventTriggers200Response.from_json(json)
# print the JSON string representation of the object
print(WebhooksGetAllEventTriggers200Response.to_json())

# convert the object into a dict
webhooks_get_all_event_triggers200_response_dict = webhooks_get_all_event_triggers200_response_instance.to_dict()
# create an instance of WebhooksGetAllEventTriggers200Response from a dict
webhooks_get_all_event_triggers200_response_from_dict = WebhooksGetAllEventTriggers200Response.from_dict(webhooks_get_all_event_triggers200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


