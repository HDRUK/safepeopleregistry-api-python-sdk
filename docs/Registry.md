# Registry

Registry model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**deleted_at** | **str** |  | [optional] 
**digi_ident** | **str** |  | [optional] 
**dl_ident** | **str** |  | [optional] 
**pp_ident** | **str** |  | [optional] 
**verified** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.registry import Registry

# TODO update the JSON string below
json = "{}"
# create an instance of Registry from a JSON string
registry_instance = Registry.from_json(json)
# print the JSON string representation of the object
print(Registry.to_json())

# convert the object into a dict
registry_dict = registry_instance.to_dict()
# create an instance of Registry from a dict
registry_from_dict = Registry.from_dict(registry_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


