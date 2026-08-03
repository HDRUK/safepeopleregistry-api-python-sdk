# Permission

Model representing permissions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the permission | [optional] 
**name** | **str** | Name of the permission | [optional] 
**enabled** | **bool** | Indicates whether the permission is enabled | [optional] 
**description** | **str** | Description of the permission | [optional] 
**created_at** | **datetime** | Timestamp when the permission was created | [optional] 
**updated_at** | **datetime** | Timestamp when the permission was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.permission import Permission

# TODO update the JSON string below
json = "{}"
# create an instance of Permission from a JSON string
permission_instance = Permission.from_json(json)
# print the JSON string representation of the object
print(Permission.to_json())

# convert the object into a dict
permission_dict = permission_instance.to_dict()
# create an instance of Permission from a dict
permission_from_dict = Permission.from_dict(permission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


