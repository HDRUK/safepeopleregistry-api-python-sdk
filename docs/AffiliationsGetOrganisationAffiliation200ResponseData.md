# AffiliationsGetOrganisationAffiliation200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**registry_id** | **int** |  | [optional] 
**organisation_id** | **int** |  | [optional] 
**model_state_id** | **int** |  | [optional] 
**model_state** | [**AffiliationsGetOrganisationAffiliation200ResponseDataModelState**](AffiliationsGetOrganisationAffiliation200ResponseDataModelState.md) |  | [optional] 
**organisation** | [**AffiliationsGetOrganisationAffiliation200ResponseDataOrganisation**](AffiliationsGetOrganisationAffiliation200ResponseDataOrganisation.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.affiliations_get_organisation_affiliation200_response_data import AffiliationsGetOrganisationAffiliation200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of AffiliationsGetOrganisationAffiliation200ResponseData from a JSON string
affiliations_get_organisation_affiliation200_response_data_instance = AffiliationsGetOrganisationAffiliation200ResponseData.from_json(json)
# print the JSON string representation of the object
print(AffiliationsGetOrganisationAffiliation200ResponseData.to_json())

# convert the object into a dict
affiliations_get_organisation_affiliation200_response_data_dict = affiliations_get_organisation_affiliation200_response_data_instance.to_dict()
# create an instance of AffiliationsGetOrganisationAffiliation200ResponseData from a dict
affiliations_get_organisation_affiliation200_response_data_from_dict = AffiliationsGetOrganisationAffiliation200ResponseData.from_dict(affiliations_get_organisation_affiliation200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


