# DecisionModelType

Model representing types of decision models

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the decision model type | [optional] 
**name** | **str** | Name of the decision model type | [optional] 
**created_at** | **datetime** | Timestamp when the decision model type was created | [optional] 
**updated_at** | **datetime** | Timestamp when the decision model type was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.decision_model_type import DecisionModelType

# TODO update the JSON string below
json = "{}"
# create an instance of DecisionModelType from a JSON string
decision_model_type_instance = DecisionModelType.from_json(json)
# print the JSON string representation of the object
print(DecisionModelType.to_json())

# convert the object into a dict
decision_model_type_dict = decision_model_type_instance.to_dict()
# create an instance of DecisionModelType from a dict
decision_model_type_from_dict = DecisionModelType.from_dict(decision_model_type_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


