# ProjectIndex200ResponseData


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

## Example

```python
from safepeopleregistry_api_sdk.models.project_index200_response_data import ProjectIndex200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectIndex200ResponseData from a JSON string
project_index200_response_data_instance = ProjectIndex200ResponseData.from_json(json)
# print the JSON string representation of the object
print(ProjectIndex200ResponseData.to_json())

# convert the object into a dict
project_index200_response_data_dict = project_index200_response_data_instance.to_dict()
# create an instance of ProjectIndex200ResponseData from a dict
project_index200_response_data_from_dict = ProjectIndex200ResponseData.from_dict(project_index200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


