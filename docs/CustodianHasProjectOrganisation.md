# CustodianHasProjectOrganisation

Custodian approval status for a project organisation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] [readonly] 
**project_has_organisation_id** | **int** | ID of the project organisation | 
**custodian_id** | **int** | ID of the custodian | 
**approved** | **bool** | Approval flag | [optional] 
**comment** | **str** | Optional comment | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 
**project_organisation** | [**ProjectHasOrganisation**](ProjectHasOrganisation.md) |  | [optional] 
**custodian** | [**Custodian**](Custodian.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_has_project_organisation import CustodianHasProjectOrganisation

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianHasProjectOrganisation from a JSON string
custodian_has_project_organisation_instance = CustodianHasProjectOrganisation.from_json(json)
# print the JSON string representation of the object
print(CustodianHasProjectOrganisation.to_json())

# convert the object into a dict
custodian_has_project_organisation_dict = custodian_has_project_organisation_instance.to_dict()
# create an instance of CustodianHasProjectOrganisation from a dict
custodian_has_project_organisation_from_dict = CustodianHasProjectOrganisation.from_dict(custodian_has_project_organisation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


