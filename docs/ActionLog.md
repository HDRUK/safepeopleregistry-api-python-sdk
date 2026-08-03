# ActionLog

Action Log model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**entity_type** | **str** | Type of the entity associated with the action log | [optional] 
**entity_id** | **int** | ID of the entity associated with the action log | [optional] 
**action** | **str** | Description of the action performed | [optional] 
**completed_at** | **datetime** | Timestamp when the action was completed (nullable) | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.action_log import ActionLog

# TODO update the JSON string below
json = "{}"
# create an instance of ActionLog from a JSON string
action_log_instance = ActionLog.from_json(json)
# print the JSON string representation of the object
print(ActionLog.to_json())

# convert the object into a dict
action_log_dict = action_log_instance.to_dict()
# create an instance of ActionLog from a dict
action_log_from_dict = ActionLog.from_dict(action_log_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


