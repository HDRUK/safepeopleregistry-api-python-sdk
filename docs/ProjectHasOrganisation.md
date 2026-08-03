# ProjectHasOrganisation

Relation between a project and an organisation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**project_id** | **int** | ID of the related project | 
**organisation_id** | **int** | ID of the related organisation | 
**organisation** | [**Organisation**](Organisation.md) |  | [optional] 
**project** | [**Project**](Project.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.project_has_organisation import ProjectHasOrganisation

# TODO update the JSON string below
json = "{}"
# create an instance of ProjectHasOrganisation from a JSON string
project_has_organisation_instance = ProjectHasOrganisation.from_json(json)
# print the JSON string representation of the object
print(ProjectHasOrganisation.to_json())

# convert the object into a dict
project_has_organisation_dict = project_has_organisation_instance.to_dict()
# create an instance of ProjectHasOrganisation from a dict
project_has_organisation_from_dict = ProjectHasOrganisation.from_dict(project_has_organisation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


