# RegistryHasEducation

Pivot model representing the relationship between registries and educations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**registry_id** | **int** | ID of the registry | [optional] 
**education_id** | **int** | ID of the education | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.registry_has_education import RegistryHasEducation

# TODO update the JSON string below
json = "{}"
# create an instance of RegistryHasEducation from a JSON string
registry_has_education_instance = RegistryHasEducation.from_json(json)
# print the JSON string representation of the object
print(RegistryHasEducation.to_json())

# convert the object into a dict
registry_has_education_dict = registry_has_education_instance.to_dict()
# create an instance of RegistryHasEducation from a dict
registry_has_education_from_dict = RegistryHasEducation.from_dict(registry_has_education_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


