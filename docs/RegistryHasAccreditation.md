# RegistryHasAccreditation

Pivot model representing the relationship between registries and accreditations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**registry_id** | **int** | ID of the registry | [optional] 
**accreditation_id** | **int** | ID of the accreditation | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.registry_has_accreditation import RegistryHasAccreditation

# TODO update the JSON string below
json = "{}"
# create an instance of RegistryHasAccreditation from a JSON string
registry_has_accreditation_instance = RegistryHasAccreditation.from_json(json)
# print the JSON string representation of the object
print(RegistryHasAccreditation.to_json())

# convert the object into a dict
registry_has_accreditation_dict = registry_has_accreditation_instance.to_dict()
# create an instance of RegistryHasAccreditation from a dict
registry_has_accreditation_from_dict = RegistryHasAccreditation.from_dict(registry_has_accreditation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


