# CustodianUserHasPermission

Model representing the relationship between Custodian Users and Permissions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**custodian_user_id** | **int** | ID of the custodian user | [optional] 
**permission_id** | **int** | ID of the permission | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_user_has_permission import CustodianUserHasPermission

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianUserHasPermission from a JSON string
custodian_user_has_permission_instance = CustodianUserHasPermission.from_json(json)
# print the JSON string representation of the object
print(CustodianUserHasPermission.to_json())

# convert the object into a dict
custodian_user_has_permission_dict = custodian_user_has_permission_instance.to_dict()
# create an instance of CustodianUserHasPermission from a dict
custodian_user_has_permission_from_dict = CustodianUserHasPermission.from_dict(custodian_user_has_permission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


