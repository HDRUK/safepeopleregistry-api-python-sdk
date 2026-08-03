# PermissionIndex200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**name** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.permission_index200_response_data import PermissionIndex200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of PermissionIndex200ResponseData from a JSON string
permission_index200_response_data_instance = PermissionIndex200ResponseData.from_json(json)
# print the JSON string representation of the object
print(PermissionIndex200ResponseData.to_json())

# convert the object into a dict
permission_index200_response_data_dict = permission_index200_response_data_instance.to_dict()
# create an instance of PermissionIndex200ResponseData from a dict
permission_index200_response_data_from_dict = PermissionIndex200ResponseData.from_dict(permission_index200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


