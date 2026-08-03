# AffiliationsGetOrganisationAffiliation200ResponseDataOrganisation


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**organisation_name** | **str** |  | [optional] 
**unclaimed** | **bool** |  | [optional] 
**lead_applicant_email** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.affiliations_get_organisation_affiliation200_response_data_organisation import AffiliationsGetOrganisationAffiliation200ResponseDataOrganisation

# TODO update the JSON string below
json = "{}"
# create an instance of AffiliationsGetOrganisationAffiliation200ResponseDataOrganisation from a JSON string
affiliations_get_organisation_affiliation200_response_data_organisation_instance = AffiliationsGetOrganisationAffiliation200ResponseDataOrganisation.from_json(json)
# print the JSON string representation of the object
print(AffiliationsGetOrganisationAffiliation200ResponseDataOrganisation.to_json())

# convert the object into a dict
affiliations_get_organisation_affiliation200_response_data_organisation_dict = affiliations_get_organisation_affiliation200_response_data_organisation_instance.to_dict()
# create an instance of AffiliationsGetOrganisationAffiliation200ResponseDataOrganisation from a dict
affiliations_get_organisation_affiliation200_response_data_organisation_from_dict = AffiliationsGetOrganisationAffiliation200ResponseDataOrganisation.from_dict(affiliations_get_organisation_affiliation200_response_data_organisation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


