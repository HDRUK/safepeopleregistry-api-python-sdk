# ProjectUpdate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**ProjectUpdate200ResponseData**](ProjectUpdate200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_update200_response import ProjectUpdate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectUpdate200Response from a JSON string
project_update200_response_instance = ProjectUpdate200Response.from_json(json)
# print the JSON string representation of the object
print(ProjectUpdate200Response.to_json())

# convert the object into a dict
project_update200_response_dict = project_update200_response_instance.to_dict()
# create an instance of ProjectUpdate200Response from a dict
project_update200_response_from_dict = ProjectUpdate200Response.from_dict(project_update200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


