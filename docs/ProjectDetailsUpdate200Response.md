# ProjectDetailsUpdate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**ProjectDetail**](ProjectDetail.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_details_update200_response import ProjectDetailsUpdate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectDetailsUpdate200Response from a JSON string
project_details_update200_response_instance = ProjectDetailsUpdate200Response.from_json(json)
# print the JSON string representation of the object
print(ProjectDetailsUpdate200Response.to_json())

# convert the object into a dict
project_details_update200_response_dict = project_details_update200_response_instance.to_dict()
# create an instance of ProjectDetailsUpdate200Response from a dict
project_details_update200_response_from_dict = ProjectDetailsUpdate200Response.from_dict(project_details_update200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


