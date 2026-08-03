# OrganisationsInviteUserRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**last_name** | **str** |  | [optional] 
**first_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**is_delegate** | **int** |  | [optional] 
**department_id** | **int** |  | [optional] 
**role** | **str** |  | [optional] 
**user_group** | **str** |  | [optional] 
**from_custodian** | **bool** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisations_invite_user_request import OrganisationsInviteUserRequest

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationsInviteUserRequest from a JSON string
organisations_invite_user_request_instance = OrganisationsInviteUserRequest.from_json(json)
# print the JSON string representation of the object
print(OrganisationsInviteUserRequest.to_json())

# convert the object into a dict
organisations_invite_user_request_dict = organisations_invite_user_request_instance.to_dict()
# create an instance of OrganisationsInviteUserRequest from a dict
organisations_invite_user_request_from_dict = OrganisationsInviteUserRequest.from_dict(organisations_invite_user_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


