# DebugLog

Model representing debug logs

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the debug log | [optional] 
**var_class** | **str** | Class name where the log was generated | [optional] 
**log** | **str** | Log message | [optional] 
**created_at** | **datetime** | Timestamp when the log was created | [optional] 
**updated_at** | **datetime** | Timestamp when the log was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.debug_log import DebugLog

# TODO update the JSON string below
json = "{}"
# create an instance of DebugLog from a JSON string
debug_log_instance = DebugLog.from_json(json)
# print the JSON string representation of the object
print(DebugLog.to_json())

# convert the object into a dict
debug_log_dict = debug_log_instance.to_dict()
# create an instance of DebugLog from a dict
debug_log_from_dict = DebugLog.from_dict(debug_log_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


