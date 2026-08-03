# CustodianProjectOrganisationsUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**approved** | **bool** | Approval status | [optional] 
**comment** | **str** | Optional comment | [optional] 
**status** | **str** | Workflow state | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_project_organisations_update_request import CustodianProjectOrganisationsUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianProjectOrganisationsUpdateRequest from a JSON string
custodian_project_organisations_update_request_instance = CustodianProjectOrganisationsUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(CustodianProjectOrganisationsUpdateRequest.to_json())

# convert the object into a dict
custodian_project_organisations_update_request_dict = custodian_project_organisations_update_request_instance.to_dict()
# create an instance of CustodianProjectOrganisationsUpdateRequest from a dict
custodian_project_organisations_update_request_from_dict = CustodianProjectOrganisationsUpdateRequest.from_dict(custodian_project_organisations_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


