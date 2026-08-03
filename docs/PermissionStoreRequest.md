# PermissionStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**enabled** | **bool** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.permission_store_request import PermissionStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PermissionStoreRequest from a JSON string
permission_store_request_instance = PermissionStoreRequest.from_json(json)
# print the JSON string representation of the object
print(PermissionStoreRequest.to_json())

# convert the object into a dict
permission_store_request_dict = permission_store_request_instance.to_dict()
# create an instance of PermissionStoreRequest from a dict
permission_store_request_from_dict = PermissionStoreRequest.from_dict(permission_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


