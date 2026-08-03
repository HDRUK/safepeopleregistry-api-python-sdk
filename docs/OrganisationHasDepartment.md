# OrganisationHasDepartment

Pivot model representing the relationship between organisations and departments

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**organisation_id** | **int** | ID of the organisation | [optional] 
**department_id** | **int** | ID of the department | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisation_has_department import OrganisationHasDepartment

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationHasDepartment from a JSON string
organisation_has_department_instance = OrganisationHasDepartment.from_json(json)
# print the JSON string representation of the object
print(OrganisationHasDepartment.to_json())

# convert the object into a dict
organisation_has_department_dict = organisation_has_department_instance.to_dict()
# create an instance of OrganisationHasDepartment from a dict
organisation_has_department_from_dict = OrganisationHasDepartment.from_dict(organisation_has_department_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


