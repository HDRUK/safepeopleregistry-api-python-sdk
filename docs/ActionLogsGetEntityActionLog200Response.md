# ActionLogsGetEntityActionLog200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**data** | [**List[ActionLog]**](ActionLog.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.action_logs_get_entity_action_log200_response import ActionLogsGetEntityActionLog200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ActionLogsGetEntityActionLog200Response from a JSON string
action_logs_get_entity_action_log200_response_instance = ActionLogsGetEntityActionLog200Response.from_json(json)
# print the JSON string representation of the object
print(ActionLogsGetEntityActionLog200Response.to_json())

# convert the object into a dict
action_logs_get_entity_action_log200_response_dict = action_logs_get_entity_action_log200_response_instance.to_dict()
# create an instance of ActionLogsGetEntityActionLog200Response from a dict
action_logs_get_entity_action_log200_response_from_dict = ActionLogsGetEntityActionLog200Response.from_dict(action_logs_get_entity_action_log200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


