# ProjectGetProjectUsers200ResponseDataInnerRegistryUser


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**registry_id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**user_group** | **str** |  | [optional] 
**consent_scrape** | **bool** |  | [optional] 
**public_opt_in** | **bool** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_get_project_users200_response_data_inner_registry_user import ProjectGetProjectUsers200ResponseDataInnerRegistryUser

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectGetProjectUsers200ResponseDataInnerRegistryUser from a JSON string
project_get_project_users200_response_data_inner_registry_user_instance = ProjectGetProjectUsers200ResponseDataInnerRegistryUser.from_json(json)
# print the JSON string representation of the object
print(ProjectGetProjectUsers200ResponseDataInnerRegistryUser.to_json())

# convert the object into a dict
project_get_project_users200_response_data_inner_registry_user_dict = project_get_project_users200_response_data_inner_registry_user_instance.to_dict()
# create an instance of ProjectGetProjectUsers200ResponseDataInnerRegistryUser from a dict
project_get_project_users200_response_data_inner_registry_user_from_dict = ProjectGetProjectUsers200ResponseDataInnerRegistryUser.from_dict(project_get_project_users200_response_data_inner_registry_user_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


