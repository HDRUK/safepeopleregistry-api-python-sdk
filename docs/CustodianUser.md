# CustodianUser

CustodianUser model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**custodian_id** | **int** | Custodian primary key | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_user import CustodianUser

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianUser from a JSON string
custodian_user_instance = CustodianUser.from_json(json)
# print the JSON string representation of the object
print(CustodianUser.to_json())

# convert the object into a dict
custodian_user_dict = custodian_user_instance.to_dict()
# create an instance of CustodianUser from a dict
custodian_user_from_dict = CustodianUser.from_dict(custodian_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


