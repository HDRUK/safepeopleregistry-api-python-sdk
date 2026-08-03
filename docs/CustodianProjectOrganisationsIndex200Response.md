# CustodianProjectOrganisationsIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[CustodianHasProjectOrganisation]**](CustodianHasProjectOrganisation.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_project_organisations_index200_response import CustodianProjectOrganisationsIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianProjectOrganisationsIndex200Response from a JSON string
custodian_project_organisations_index200_response_instance = CustodianProjectOrganisationsIndex200Response.from_json(json)
# print the JSON string representation of the object
print(CustodianProjectOrganisationsIndex200Response.to_json())

# convert the object into a dict
custodian_project_organisations_index200_response_dict = custodian_project_organisations_index200_response_instance.to_dict()
# create an instance of CustodianProjectOrganisationsIndex200Response from a dict
custodian_project_organisations_index200_response_from_dict = CustodianProjectOrganisationsIndex200Response.from_dict(custodian_project_organisations_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


