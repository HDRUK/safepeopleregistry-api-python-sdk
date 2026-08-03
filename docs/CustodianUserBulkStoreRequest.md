# CustodianUserBulkStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**users** | [**List[CustodianUserBulkStoreRequestUsersInner]**](CustodianUserBulkStoreRequestUsersInner.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_user_bulk_store_request import CustodianUserBulkStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianUserBulkStoreRequest from a JSON string
custodian_user_bulk_store_request_instance = CustodianUserBulkStoreRequest.from_json(json)
# print the JSON string representation of the object
print(CustodianUserBulkStoreRequest.to_json())

# convert the object into a dict
custodian_user_bulk_store_request_dict = custodian_user_bulk_store_request_instance.to_dict()
# create an instance of CustodianUserBulkStoreRequest from a dict
custodian_user_bulk_store_request_from_dict = CustodianUserBulkStoreRequest.from_dict(custodian_user_bulk_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


