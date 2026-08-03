# DecisionModel

Model representing decision models

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the decision model | [optional] 
**model_type** | **str** | Type of the model associated with the decision | 
**conditions** | **str** | Conditions for the decision model | 
**rule_class** | **str** | Class defining the rules for the decision model | 
**description** | **str** | Description of the decision model | [optional] 
**entity_model_type_id** | **int** | ID of the entity model type associated with the decision | [optional] 
**created_at** | **datetime** | Timestamp when the decision model was created | [optional] 
**updated_at** | **datetime** | Timestamp when the decision model was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.decision_model import DecisionModel

# TODO update the JSON string below
json = "{}"
# create an instance of DecisionModel from a JSON string
decision_model_instance = DecisionModel.from_json(json)
# print the JSON string representation of the object
print(DecisionModel.to_json())

# convert the object into a dict
decision_model_dict = decision_model_instance.to_dict()
# create an instance of DecisionModel from a dict
decision_model_from_dict = DecisionModel.from_dict(decision_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


