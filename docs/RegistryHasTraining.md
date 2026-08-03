# RegistryHasTraining

Pivot model representing the relationship between registries and trainings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**registry_id** | **int** | ID of the registry | [optional] 
**training_id** | **int** | ID of the training | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.registry_has_training import RegistryHasTraining

# TODO update the JSON string below
json = "{}"
# create an instance of RegistryHasTraining from a JSON string
registry_has_training_instance = RegistryHasTraining.from_json(json)
# print the JSON string representation of the object
print(RegistryHasTraining.to_json())

# convert the object into a dict
registry_has_training_dict = registry_has_training_instance.to_dict()
# create an instance of RegistryHasTraining from a dict
registry_has_training_from_dict = RegistryHasTraining.from_dict(registry_has_training_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


