# ProjectDetailIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**ProjectDetail**](ProjectDetail.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_detail_index200_response import ProjectDetailIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectDetailIndex200Response from a JSON string
project_detail_index200_response_instance = ProjectDetailIndex200Response.from_json(json)
# print the JSON string representation of the object
print(ProjectDetailIndex200Response.to_json())

# convert the object into a dict
project_detail_index200_response_dict = project_detail_index200_response_instance.to_dict()
# create an instance of ProjectDetailIndex200Response from a dict
project_detail_index200_response_from_dict = ProjectDetailIndex200Response.from_dict(project_detail_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


