# ProjectRole

ProjectRole model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**name** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_role import ProjectRole

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectRole from a JSON string
project_role_instance = ProjectRole.from_json(json)
# print the JSON string representation of the object
print(ProjectRole.to_json())

# convert the object into a dict
project_role_dict = project_role_instance.to_dict()
# create an instance of ProjectRole from a dict
project_role_from_dict = ProjectRole.from_dict(project_role_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


