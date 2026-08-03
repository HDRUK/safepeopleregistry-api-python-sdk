# RegistryHasAffiliation

Pivot model representing the relationship between registries and affiliations

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the registry-affiliation relationship | [optional] 
**registry_id** | **int** | ID of the registry | [optional] 
**affiliation_id** | **int** | ID of the affiliation | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.registry_has_affiliation import RegistryHasAffiliation

# TODO update the JSON string below
json = "{}"
# create an instance of RegistryHasAffiliation from a JSON string
registry_has_affiliation_instance = RegistryHasAffiliation.from_json(json)
# print the JSON string representation of the object
print(RegistryHasAffiliation.to_json())

# convert the object into a dict
registry_has_affiliation_dict = registry_has_affiliation_instance.to_dict()
# create an instance of RegistryHasAffiliation from a dict
registry_has_affiliation_from_dict = RegistryHasAffiliation.from_dict(registry_has_affiliation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


