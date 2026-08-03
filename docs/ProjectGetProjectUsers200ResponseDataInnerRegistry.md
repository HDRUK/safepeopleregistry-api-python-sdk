# ProjectGetProjectUsers200ResponseDataInnerRegistry


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**verified** | **bool** |  | [optional] 
**user** | [**ProjectGetProjectUsers200ResponseDataInnerRegistryUser**](ProjectGetProjectUsers200ResponseDataInnerRegistryUser.md) |  | [optional] 
**organisations** | [**List[ProjectGetProjectUsers200ResponseDataInnerRegistryOrganisationsInner]**](ProjectGetProjectUsers200ResponseDataInnerRegistryOrganisationsInner.md) |  | [optional] 
**affiliation** | [**ProjectGetProjectUsers200ResponseDataInnerRegistryAffiliation**](ProjectGetProjectUsers200ResponseDataInnerRegistryAffiliation.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_get_project_users200_response_data_inner_registry import ProjectGetProjectUsers200ResponseDataInnerRegistry

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectGetProjectUsers200ResponseDataInnerRegistry from a JSON string
project_get_project_users200_response_data_inner_registry_instance = ProjectGetProjectUsers200ResponseDataInnerRegistry.from_json(json)
# print the JSON string representation of the object
print(ProjectGetProjectUsers200ResponseDataInnerRegistry.to_json())

# convert the object into a dict
project_get_project_users200_response_data_inner_registry_dict = project_get_project_users200_response_data_inner_registry_instance.to_dict()
# create an instance of ProjectGetProjectUsers200ResponseDataInnerRegistry from a dict
project_get_project_users200_response_data_inner_registry_from_dict = ProjectGetProjectUsers200ResponseDataInnerRegistry.from_dict(project_get_project_users200_response_data_inner_registry_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


