# ProjectGetAllUsersFlagProjectByUserId200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[ProjectGetAllUsersFlagProjectByUserId200ResponseDataInner]**](ProjectGetAllUsersFlagProjectByUserId200ResponseDataInner.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_get_all_users_flag_project_by_user_id200_response import ProjectGetAllUsersFlagProjectByUserId200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectGetAllUsersFlagProjectByUserId200Response from a JSON string
project_get_all_users_flag_project_by_user_id200_response_instance = ProjectGetAllUsersFlagProjectByUserId200Response.from_json(json)
# print the JSON string representation of the object
print(ProjectGetAllUsersFlagProjectByUserId200Response.to_json())

# convert the object into a dict
project_get_all_users_flag_project_by_user_id200_response_dict = project_get_all_users_flag_project_by_user_id200_response_instance.to_dict()
# create an instance of ProjectGetAllUsersFlagProjectByUserId200Response from a dict
project_get_all_users_flag_project_by_user_id200_response_from_dict = ProjectGetAllUsersFlagProjectByUserId200Response.from_dict(project_get_all_users_flag_project_by_user_id200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


