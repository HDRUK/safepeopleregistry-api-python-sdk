# AffiliationsGetOrganisationAffiliation200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**AffiliationsGetOrganisationAffiliation200ResponseData**](AffiliationsGetOrganisationAffiliation200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.affiliations_get_organisation_affiliation200_response import AffiliationsGetOrganisationAffiliation200Response

# TODO update the JSON string below
json = "{}"
# create an instance of AffiliationsGetOrganisationAffiliation200Response from a JSON string
affiliations_get_organisation_affiliation200_response_instance = AffiliationsGetOrganisationAffiliation200Response.from_json(json)
# print the JSON string representation of the object
print(AffiliationsGetOrganisationAffiliation200Response.to_json())

# convert the object into a dict
affiliations_get_organisation_affiliation200_response_dict = affiliations_get_organisation_affiliation200_response_instance.to_dict()
# create an instance of AffiliationsGetOrganisationAffiliation200Response from a dict
affiliations_get_organisation_affiliation200_response_from_dict = AffiliationsGetOrganisationAffiliation200Response.from_dict(affiliations_get_organisation_affiliation200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


