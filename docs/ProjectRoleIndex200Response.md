# ProjectRoleIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**ProjectRole**](ProjectRole.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_role_index200_response import ProjectRoleIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectRoleIndex200Response from a JSON string
project_role_index200_response_instance = ProjectRoleIndex200Response.from_json(json)
# print the JSON string representation of the object
print(ProjectRoleIndex200Response.to_json())

# convert the object into a dict
project_role_index200_response_dict = project_role_index200_response_instance.to_dict()
# create an instance of ProjectRoleIndex200Response from a dict
project_role_index200_response_from_dict = ProjectRoleIndex200Response.from_dict(project_role_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


