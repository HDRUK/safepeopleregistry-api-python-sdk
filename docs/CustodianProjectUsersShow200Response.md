# CustodianProjectUsersShow200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**CustodianHasProjectUser**](CustodianHasProjectUser.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_project_users_show200_response import CustodianProjectUsersShow200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianProjectUsersShow200Response from a JSON string
custodian_project_users_show200_response_instance = CustodianProjectUsersShow200Response.from_json(json)
# print the JSON string representation of the object
print(CustodianProjectUsersShow200Response.to_json())

# convert the object into a dict
custodian_project_users_show200_response_dict = custodian_project_users_show200_response_instance.to_dict()
# create an instance of CustodianProjectUsersShow200Response from a dict
custodian_project_users_show200_response_from_dict = CustodianProjectUsersShow200Response.from_dict(custodian_project_users_show200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


