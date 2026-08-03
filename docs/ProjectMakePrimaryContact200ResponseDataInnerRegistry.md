# ProjectMakePrimaryContact200ResponseDataInnerRegistry


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**verified** | **bool** |  | [optional] 
**user** | [**ProjectGetProjectUsers200ResponseDataInnerRegistryUser**](ProjectGetProjectUsers200ResponseDataInnerRegistryUser.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_make_primary_contact200_response_data_inner_registry import ProjectMakePrimaryContact200ResponseDataInnerRegistry

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectMakePrimaryContact200ResponseDataInnerRegistry from a JSON string
project_make_primary_contact200_response_data_inner_registry_instance = ProjectMakePrimaryContact200ResponseDataInnerRegistry.from_json(json)
# print the JSON string representation of the object
print(ProjectMakePrimaryContact200ResponseDataInnerRegistry.to_json())

# convert the object into a dict
project_make_primary_contact200_response_data_inner_registry_dict = project_make_primary_contact200_response_data_inner_registry_instance.to_dict()
# create an instance of ProjectMakePrimaryContact200ResponseDataInnerRegistry from a dict
project_make_primary_contact200_response_data_inner_registry_from_dict = ProjectMakePrimaryContact200ResponseDataInnerRegistry.from_dict(project_make_primary_contact200_response_data_inner_registry_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


