# CustodianProjectUsersUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**approved** | **bool** | Approval status | [optional] 
**comment** | **str** | Optional comment | [optional] 
**status** | **str** | State machine status | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_project_users_update_request import CustodianProjectUsersUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianProjectUsersUpdateRequest from a JSON string
custodian_project_users_update_request_instance = CustodianProjectUsersUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(CustodianProjectUsersUpdateRequest.to_json())

# convert the object into a dict
custodian_project_users_update_request_dict = custodian_project_users_update_request_instance.to_dict()
# create an instance of CustodianProjectUsersUpdateRequest from a dict
custodian_project_users_update_request_from_dict = CustodianProjectUsersUpdateRequest.from_dict(custodian_project_users_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


