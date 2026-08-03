# UserHasCustodianPermission

Pivot model representing the relationship between users, custodians, and permissions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**user_id** | **int** | ID of the user | [optional] 
**permission_id** | **int** | ID of the permission | [optional] 
**custodian_id** | **int** | ID of the custodian | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.user_has_custodian_permission import UserHasCustodianPermission

# TODO update the JSON string below
json = "{}"
# create an instance of UserHasCustodianPermission from a JSON string
user_has_custodian_permission_instance = UserHasCustodianPermission.from_json(json)
# print the JSON string representation of the object
print(UserHasCustodianPermission.to_json())

# convert the object into a dict
user_has_custodian_permission_dict = user_has_custodian_permission_instance.to_dict()
# create an instance of UserHasCustodianPermission from a dict
user_has_custodian_permission_from_dict = UserHasCustodianPermission.from_dict(user_has_custodian_permission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


