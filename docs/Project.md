# Project

Project model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**title** | **str** |  | [optional] 
**unique_id** | **str** |  | [optional] 
**lay_summary** | **str** |  | [optional] 
**public_benefit** | **str** | A unique identifier for Custodian&#39;s within SOURSD | [optional] 
**request_category_type** | **str** |  | [optional] 
**technical_summary** | **str** |  | [optional] 
**other_approval_commitees** | **str** |  | [optional] 
**start_date** | **str** |  | [optional] 
**end_date** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project import Project

# TODO update the JSON string below
json = "{}"
# create an instance of Project from a JSON string
project_instance = Project.from_json(json)
# print the JSON string representation of the object
print(Project.to_json())

# convert the object into a dict
project_dict = project_instance.to_dict()
# create an instance of Project from a dict
project_from_dict = Project.from_dict(project_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


