# ProjectUpdateAllProjectUsersRequestUsersInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**registry_id** | **int** |  | [optional] 
**affiliation_id** | **int** |  | [optional] 
**project_user_id** | **int** |  | [optional] 
**primary_contact** | **bool** |  | [optional] 
**role** | [**ProjectUpdateAllProjectUsersRequestUsersInnerRole**](ProjectUpdateAllProjectUsersRequestUsersInnerRole.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_update_all_project_users_request_users_inner import ProjectUpdateAllProjectUsersRequestUsersInner

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectUpdateAllProjectUsersRequestUsersInner from a JSON string
project_update_all_project_users_request_users_inner_instance = ProjectUpdateAllProjectUsersRequestUsersInner.from_json(json)
# print the JSON string representation of the object
print(ProjectUpdateAllProjectUsersRequestUsersInner.to_json())

# convert the object into a dict
project_update_all_project_users_request_users_inner_dict = project_update_all_project_users_request_users_inner_instance.to_dict()
# create an instance of ProjectUpdateAllProjectUsersRequestUsersInner from a dict
project_update_all_project_users_request_users_inner_from_dict = ProjectUpdateAllProjectUsersRequestUsersInner.from_dict(project_update_all_project_users_request_users_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


