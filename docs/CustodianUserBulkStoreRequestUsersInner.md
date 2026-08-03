# CustodianUserBulkStoreRequestUsersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**permission** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_user_bulk_store_request_users_inner import CustodianUserBulkStoreRequestUsersInner

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianUserBulkStoreRequestUsersInner from a JSON string
custodian_user_bulk_store_request_users_inner_instance = CustodianUserBulkStoreRequestUsersInner.from_json(json)
# print the JSON string representation of the object
print(CustodianUserBulkStoreRequestUsersInner.to_json())

# convert the object into a dict
custodian_user_bulk_store_request_users_inner_dict = custodian_user_bulk_store_request_users_inner_instance.to_dict()
# create an instance of CustodianUserBulkStoreRequestUsersInner from a dict
custodian_user_bulk_store_request_users_inner_from_dict = CustodianUserBulkStoreRequestUsersInner.from_dict(custodian_user_bulk_store_request_users_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


