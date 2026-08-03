# ProjectDetail

ProjectDetail model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**project_id** | **int** | Primary key of associated Project for this ProjectDetail | [optional] 
**datasets** | **List[str]** |  | [optional] 
**other_approval_committees** | **List[str]** |  | [optional] 
**data_sensitivity_level** | **str** |  | [optional] 
**legal_basis_for_data_article6** | **str** |  | [optional] 
**duty_of_confidentiality** | **bool** |  | [optional] 
**national_data_optout** | **bool** |  | [optional] 
**request_frequency** | **str** |  | [optional] 
**dataset_linkage_description** | **str** |  | [optional] 
**data_minimisation** | **str** |  | [optional] 
**data_use_description** | **str** |  | [optional] 
**access_date** | **str** |  | [optional] 
**access_type** | **int** |  | [optional] 
**data_privacy** | **str** |  | [optional] 
**research_outputs** | **object** |  | [optional] 
**data_assets** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_detail import ProjectDetail

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectDetail from a JSON string
project_detail_instance = ProjectDetail.from_json(json)
# print the JSON string representation of the object
print(ProjectDetail.to_json())

# convert the object into a dict
project_detail_dict = project_detail_instance.to_dict()
# create an instance of ProjectDetail from a dict
project_detail_from_dict = ProjectDetail.from_dict(project_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


