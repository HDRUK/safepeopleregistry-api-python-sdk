# ProjectUpdate200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**registry_id** | **int** |  | [optional] 
**name** | **str** |  | [optional] 
**public_benefit** | **str** |  | [optional] 
**runs_to** | **str** |  | [optional] 
**status** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_update200_response_data import ProjectUpdate200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectUpdate200ResponseData from a JSON string
project_update200_response_data_instance = ProjectUpdate200ResponseData.from_json(json)
# print the JSON string representation of the object
print(ProjectUpdate200ResponseData.to_json())

# convert the object into a dict
project_update200_response_data_dict = project_update200_response_data_instance.to_dict()
# create an instance of ProjectUpdate200ResponseData from a dict
project_update200_response_data_from_dict = ProjectUpdate200ResponseData.from_dict(project_update200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


