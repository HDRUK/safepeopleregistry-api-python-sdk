# CustodianHasProjectUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**project_has_user_id** | **int** |  | [optional] 
**custodian_id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**project_has_user** | [**ProjectHasUser**](ProjectHasUser.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_has_project_user import CustodianHasProjectUser

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianHasProjectUser from a JSON string
custodian_has_project_user_instance = CustodianHasProjectUser.from_json(json)
# print the JSON string representation of the object
print(CustodianHasProjectUser.to_json())

# convert the object into a dict
custodian_has_project_user_dict = custodian_has_project_user_instance.to_dict()
# create an instance of CustodianHasProjectUser from a dict
custodian_has_project_user_from_dict = CustodianHasProjectUser.from_dict(custodian_has_project_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


