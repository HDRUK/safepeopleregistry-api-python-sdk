# ProjectUsersBulkInviteProjectUsersRequestUsersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email_address** | **str** |  | [optional] 
**project_role** | **str** |  | [optional] 
**organisation_id** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_users_bulk_invite_project_users_request_users_inner import ProjectUsersBulkInviteProjectUsersRequestUsersInner

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectUsersBulkInviteProjectUsersRequestUsersInner from a JSON string
project_users_bulk_invite_project_users_request_users_inner_instance = ProjectUsersBulkInviteProjectUsersRequestUsersInner.from_json(json)
# print the JSON string representation of the object
print(ProjectUsersBulkInviteProjectUsersRequestUsersInner.to_json())

# convert the object into a dict
project_users_bulk_invite_project_users_request_users_inner_dict = project_users_bulk_invite_project_users_request_users_inner_instance.to_dict()
# create an instance of ProjectUsersBulkInviteProjectUsersRequestUsersInner from a dict
project_users_bulk_invite_project_users_request_users_inner_from_dict = ProjectUsersBulkInviteProjectUsersRequestUsersInner.from_dict(project_users_bulk_invite_project_users_request_users_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


