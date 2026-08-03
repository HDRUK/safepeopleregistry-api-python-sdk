# ModelState

Model representing the state of a model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the model state | [optional] 
**state_id** | **int** | ID of the state associated with the model state | [optional] 
**stateable_type** | **str** | Type of the model associated with the state | [optional] 
**stateable_id** | **int** | ID of the model associated with the state | [optional] 
**created_at** | **datetime** | Timestamp when the model state was created | [optional] 
**updated_at** | **datetime** | Timestamp when the model state was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.model_state import ModelState

# TODO update the JSON string below
json = "{}"
# create an instance of ModelState from a JSON string
model_state_instance = ModelState.from_json(json)
# print the JSON string representation of the object
print(ModelState.to_json())

# convert the object into a dict
model_state_dict = model_state_instance.to_dict()
# create an instance of ModelState from a dict
model_state_from_dict = ModelState.from_dict(model_state_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


