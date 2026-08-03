# State

Model representing states

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the state | [optional] 
**name** | **str** | Name of the state | [optional] 
**slug** | **str** | Slug identifier for the state | [optional] 
**created_at** | **datetime** | Timestamp when the state was created | [optional] 
**updated_at** | **datetime** | Timestamp when the state was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.state import State

# TODO update the JSON string below
json = "{}"
# create an instance of State from a JSON string
state_instance = State.from_json(json)
# print the JSON string representation of the object
print(State.to_json())

# convert the object into a dict
state_dict = state_instance.to_dict()
# create an instance of State from a dict
state_from_dict = State.from_dict(state_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


