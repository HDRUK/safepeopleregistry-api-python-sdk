# ProjectHasRole

Pivot model representing the relationship between projects and roles

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**project_id** | **int** | ID of the project | [optional] 
**project_role_id** | **int** | ID of the project role | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_has_role import ProjectHasRole

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectHasRole from a JSON string
project_has_role_instance = ProjectHasRole.from_json(json)
# print the JSON string representation of the object
print(ProjectHasRole.to_json())

# convert the object into a dict
project_has_role_dict = project_has_role_instance.to_dict()
# create an instance of ProjectHasRole from a dict
project_has_role_from_dict = ProjectHasRole.from_dict(project_has_role_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


