# ProjectGetProjectUsers200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[ProjectGetProjectUsers200ResponseDataInner]**](ProjectGetProjectUsers200ResponseDataInner.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_get_project_users200_response import ProjectGetProjectUsers200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectGetProjectUsers200Response from a JSON string
project_get_project_users200_response_instance = ProjectGetProjectUsers200Response.from_json(json)
# print the JSON string representation of the object
print(ProjectGetProjectUsers200Response.to_json())

# convert the object into a dict
project_get_project_users200_response_dict = project_get_project_users200_response_instance.to_dict()
# create an instance of ProjectGetProjectUsers200Response from a dict
project_get_project_users200_response_from_dict = ProjectGetProjectUsers200Response.from_dict(project_get_project_users200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


