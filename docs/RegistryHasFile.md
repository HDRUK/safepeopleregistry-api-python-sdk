# RegistryHasFile

Pivot model representing the relationship between registries and files

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**registry_id** | **int** | ID of the registry | [optional] 
**file_id** | **str** | ID of the file | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.registry_has_file import RegistryHasFile

# TODO update the JSON string below
json = "{}"
# create an instance of RegistryHasFile from a JSON string
registry_has_file_instance = RegistryHasFile.from_json(json)
# print the JSON string representation of the object
print(RegistryHasFile.to_json())

# convert the object into a dict
registry_has_file_dict = registry_has_file_instance.to_dict()
# create an instance of RegistryHasFile from a dict
registry_has_file_from_dict = RegistryHasFile.from_dict(registry_has_file_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


