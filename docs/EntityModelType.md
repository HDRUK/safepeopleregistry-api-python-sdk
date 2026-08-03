# EntityModelType

Model representing types of entity models

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the entity model type | [optional] 
**name** | **str** | Name of the entity model type | [optional] 
**created_at** | **datetime** | Timestamp when the entity model type was created | [optional] 
**updated_at** | **datetime** | Timestamp when the entity model type was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.entity_model_type import EntityModelType

# TODO update the JSON string below
json = "{}"
# create an instance of EntityModelType from a JSON string
entity_model_type_instance = EntityModelType.from_json(json)
# print the JSON string representation of the object
print(EntityModelType.to_json())

# convert the object into a dict
entity_model_type_dict = entity_model_type_instance.to_dict()
# create an instance of EntityModelType from a dict
entity_model_type_from_dict = EntityModelType.from_dict(entity_model_type_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


