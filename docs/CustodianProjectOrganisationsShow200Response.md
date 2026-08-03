# CustodianProjectOrganisationsShow200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**CustodianHasProjectOrganisation**](CustodianHasProjectOrganisation.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.custodian_project_organisations_show200_response import CustodianProjectOrganisationsShow200Response

# TODO update the JSON string below
json = "{}"
# create an instance of CustodianProjectOrganisationsShow200Response from a JSON string
custodian_project_organisations_show200_response_instance = CustodianProjectOrganisationsShow200Response.from_json(json)
# print the JSON string representation of the object
print(CustodianProjectOrganisationsShow200Response.to_json())

# convert the object into a dict
custodian_project_organisations_show200_response_dict = custodian_project_organisations_show200_response_instance.to_dict()
# create an instance of CustodianProjectOrganisationsShow200Response from a dict
custodian_project_organisations_show200_response_from_dict = CustodianProjectOrganisationsShow200Response.from_dict(custodian_project_organisations_show200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


