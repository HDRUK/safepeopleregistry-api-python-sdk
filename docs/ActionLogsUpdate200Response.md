# ActionLogsUpdate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**ActionLog**](ActionLog.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.action_logs_update200_response import ActionLogsUpdate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ActionLogsUpdate200Response from a JSON string
action_logs_update200_response_instance = ActionLogsUpdate200Response.from_json(json)
# print the JSON string representation of the object
print(ActionLogsUpdate200Response.to_json())

# convert the object into a dict
action_logs_update200_response_dict = action_logs_update200_response_instance.to_dict()
# create an instance of ActionLogsUpdate200Response from a dict
action_logs_update200_response_from_dict = ActionLogsUpdate200Response.from_dict(action_logs_update200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


