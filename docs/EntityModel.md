# EntityModel

Model representing entity models

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the entity model | [optional] 
**name** | **str** | Name of the entity model | [optional] 
**description** | **str** | Description of the entity model | [optional] 
**entity_model_type_id** | **int** | ID of the entity model type associated with this model | [optional] 
**calls_file** | **bool** | Indicates whether the model calls a file | [optional] 
**file_path** | **str** | Path to the file called by the model | [optional] 
**calls_operation** | **bool** | Indicates whether the model calls an operation | [optional] 
**operation** | **str** | Operation called by the model | [optional] 
**active** | **int** | Indicates whether the model is active (1 for active, 0 for inactive) | [optional] 
**created_at** | **datetime** | Timestamp when the entity model was created | [optional] 
**updated_at** | **datetime** | Timestamp when the entity model was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.entity_model import EntityModel

# TODO update the JSON string below
json = "{}"
# create an instance of EntityModel from a JSON string
entity_model_instance = EntityModel.from_json(json)
# print the JSON string representation of the object
print(EntityModel.to_json())

# convert the object into a dict
entity_model_dict = entity_model_instance.to_dict()
# create an instance of EntityModel from a dict
entity_model_from_dict = EntityModel.from_dict(entity_model_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


