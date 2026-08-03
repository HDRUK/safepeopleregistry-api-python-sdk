# ProjectGetAllUsersFlagProjectByUserId200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**project_user_id** | **int** |  | [optional] 
**user_id** | **int** |  | [optional] 
**registry_id** | **int** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**professional_email** | **str** |  | [optional] 
**affiliation_id** | **int** |  | [optional] 
**organisation_name** | **str** |  | [optional] 
**role** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_get_all_users_flag_project_by_user_id200_response_data_inner import ProjectGetAllUsersFlagProjectByUserId200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectGetAllUsersFlagProjectByUserId200ResponseDataInner from a JSON string
project_get_all_users_flag_project_by_user_id200_response_data_inner_instance = ProjectGetAllUsersFlagProjectByUserId200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(ProjectGetAllUsersFlagProjectByUserId200ResponseDataInner.to_json())

# convert the object into a dict
project_get_all_users_flag_project_by_user_id200_response_data_inner_dict = project_get_all_users_flag_project_by_user_id200_response_data_inner_instance.to_dict()
# create an instance of ProjectGetAllUsersFlagProjectByUserId200ResponseDataInner from a dict
project_get_all_users_flag_project_by_user_id200_response_data_inner_from_dict = ProjectGetAllUsersFlagProjectByUserId200ResponseDataInner.from_dict(project_get_all_users_flag_project_by_user_id200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


