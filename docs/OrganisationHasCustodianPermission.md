# OrganisationHasCustodianPermission

Pivot model representing the relationship between organisations, custodians, and permissions

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**organisation_id** | **int** | ID of the organisation | [optional] 
**permission_id** | **int** | ID of the permission | [optional] 
**custodian_id** | **int** | ID of the custodian | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisation_has_custodian_permission import OrganisationHasCustodianPermission

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationHasCustodianPermission from a JSON string
organisation_has_custodian_permission_instance = OrganisationHasCustodianPermission.from_json(json)
# print the JSON string representation of the object
print(OrganisationHasCustodianPermission.to_json())

# convert the object into a dict
organisation_has_custodian_permission_dict = organisation_has_custodian_permission_instance.to_dict()
# create an instance of OrganisationHasCustodianPermission from a dict
organisation_has_custodian_permission_from_dict = OrganisationHasCustodianPermission.from_dict(organisation_has_custodian_permission_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


