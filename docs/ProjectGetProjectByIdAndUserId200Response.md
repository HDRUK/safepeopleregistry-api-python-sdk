# ProjectGetProjectByIdAndUserId200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[Project]**](Project.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_get_project_by_id_and_user_id200_response import ProjectGetProjectByIdAndUserId200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectGetProjectByIdAndUserId200Response from a JSON string
project_get_project_by_id_and_user_id200_response_instance = ProjectGetProjectByIdAndUserId200Response.from_json(json)
# print the JSON string representation of the object
print(ProjectGetProjectByIdAndUserId200Response.to_json())

# convert the object into a dict
project_get_project_by_id_and_user_id200_response_dict = project_get_project_by_id_and_user_id200_response_instance.to_dict()
# create an instance of ProjectGetProjectByIdAndUserId200Response from a dict
project_get_project_by_id_and_user_id200_response_from_dict = ProjectGetProjectByIdAndUserId200Response.from_dict(project_get_project_by_id_and_user_id200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


