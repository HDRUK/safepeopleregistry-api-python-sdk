# ProjectUsersBulkInviteProjectUsersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**project_id** | **int** |  | 
**users** | [**List[ProjectUsersBulkInviteProjectUsersRequestUsersInner]**](ProjectUsersBulkInviteProjectUsersRequestUsersInner.md) |  | 

## Example

```python
from safepeopleregistry_api_sdk.models.project_users_bulk_invite_project_users_request import ProjectUsersBulkInviteProjectUsersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectUsersBulkInviteProjectUsersRequest from a JSON string
project_users_bulk_invite_project_users_request_instance = ProjectUsersBulkInviteProjectUsersRequest.from_json(json)
# print the JSON string representation of the object
print(ProjectUsersBulkInviteProjectUsersRequest.to_json())

# convert the object into a dict
project_users_bulk_invite_project_users_request_dict = project_users_bulk_invite_project_users_request_instance.to_dict()
# create an instance of ProjectUsersBulkInviteProjectUsersRequest from a dict
project_users_bulk_invite_project_users_request_from_dict = ProjectUsersBulkInviteProjectUsersRequest.from_dict(project_users_bulk_invite_project_users_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


