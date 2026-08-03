# CustodianProjectUsersIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[CustodianHasProjectUser]**](CustodianHasProjectUser.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_project_users_index200_response import CustodianProjectUsersIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianProjectUsersIndex200Response from a JSON string
custodian_project_users_index200_response_instance = CustodianProjectUsersIndex200Response.from_json(json)
# print the JSON string representation of the object
print(CustodianProjectUsersIndex200Response.to_json())

# convert the object into a dict
custodian_project_users_index200_response_dict = custodian_project_users_index200_response_instance.to_dict()
# create an instance of CustodianProjectUsersIndex200Response from a dict
custodian_project_users_index200_response_from_dict = CustodianProjectUsersIndex200Response.from_dict(custodian_project_users_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


