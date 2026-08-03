# RegistryHasHistory

Pivot model representing the relationship between registries and histories

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**registry_id** | **int** | ID of the registry | [optional] 
**history_id** | **int** | ID of the history | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.registry_has_history import RegistryHasHistory

# TODO update the JSON string below
json = "{}"
# create an instance of RegistryHasHistory from a JSON string
registry_has_history_instance = RegistryHasHistory.from_json(json)
# print the JSON string representation of the object
print(RegistryHasHistory.to_json())

# convert the object into a dict
registry_has_history_dict = registry_has_history_instance.to_dict()
# create an instance of RegistryHasHistory from a dict
registry_has_history_from_dict = RegistryHasHistory.from_dict(registry_has_history_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


