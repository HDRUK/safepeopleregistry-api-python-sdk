# ProjectMakePrimaryContact200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[ProjectMakePrimaryContact200ResponseDataInner]**](ProjectMakePrimaryContact200ResponseDataInner.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_make_primary_contact200_response import ProjectMakePrimaryContact200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectMakePrimaryContact200Response from a JSON string
project_make_primary_contact200_response_instance = ProjectMakePrimaryContact200Response.from_json(json)
# print the JSON string representation of the object
print(ProjectMakePrimaryContact200Response.to_json())

# convert the object into a dict
project_make_primary_contact200_response_dict = project_make_primary_contact200_response_instance.to_dict()
# create an instance of ProjectMakePrimaryContact200Response from a dict
project_make_primary_contact200_response_from_dict = ProjectMakePrimaryContact200Response.from_dict(project_make_primary_contact200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


