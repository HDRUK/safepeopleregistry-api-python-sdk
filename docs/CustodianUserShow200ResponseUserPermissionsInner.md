# CustodianUserShow200ResponseUserPermissionsInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**custodian_user_id** | **int** |  | [optional] 
**permission_id** | **int** |  | [optional] 
**permission** | [**Permission**](Permission.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_user_show200_response_user_permissions_inner import CustodianUserShow200ResponseUserPermissionsInner

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianUserShow200ResponseUserPermissionsInner from a JSON string
custodian_user_show200_response_user_permissions_inner_instance = CustodianUserShow200ResponseUserPermissionsInner.from_json(json)
# print the JSON string representation of the object
print(CustodianUserShow200ResponseUserPermissionsInner.to_json())

# convert the object into a dict
custodian_user_show200_response_user_permissions_inner_dict = custodian_user_show200_response_user_permissions_inner_instance.to_dict()
# create an instance of CustodianUserShow200ResponseUserPermissionsInner from a dict
custodian_user_show200_response_user_permissions_inner_from_dict = CustodianUserShow200ResponseUserPermissionsInner.from_dict(custodian_user_show200_response_user_permissions_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


