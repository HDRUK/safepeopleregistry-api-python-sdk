# ProjectHasCustodian

Pivot model representing the relationship between projects and custodians

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the project-custodian relationship | [optional] 
**project_id** | **int** | ID of the project | [optional] 
**custodian_id** | **int** | ID of the custodian | [optional] 
**approved** | **int** | Indicates whether the custodian is approved for the project (1 for approved, 0 for not approved) | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_has_custodian import ProjectHasCustodian

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectHasCustodian from a JSON string
project_has_custodian_instance = ProjectHasCustodian.from_json(json)
# print the JSON string representation of the object
print(ProjectHasCustodian.to_json())

# convert the object into a dict
project_has_custodian_dict = project_has_custodian_instance.to_dict()
# create an instance of ProjectHasCustodian from a dict
project_has_custodian_from_dict = ProjectHasCustodian.from_dict(project_has_custodian_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


