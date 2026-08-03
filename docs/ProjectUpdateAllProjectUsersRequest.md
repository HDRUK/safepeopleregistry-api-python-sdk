# ProjectUpdateAllProjectUsersRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**users** | [**List[ProjectUpdateAllProjectUsersRequestUsersInner]**](ProjectUpdateAllProjectUsersRequestUsersInner.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_update_all_project_users_request import ProjectUpdateAllProjectUsersRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectUpdateAllProjectUsersRequest from a JSON string
project_update_all_project_users_request_instance = ProjectUpdateAllProjectUsersRequest.from_json(json)
# print the JSON string representation of the object
print(ProjectUpdateAllProjectUsersRequest.to_json())

# convert the object into a dict
project_update_all_project_users_request_dict = project_update_all_project_users_request_instance.to_dict()
# create an instance of ProjectUpdateAllProjectUsersRequest from a dict
project_update_all_project_users_request_from_dict = ProjectUpdateAllProjectUsersRequest.from_dict(project_update_all_project_users_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


