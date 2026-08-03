# AffiliationsGetOrganisationAffiliation200ResponseDataModelState


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**state_id** | **int** |  | [optional] 
**state** | [**AffiliationsGetOrganisationAffiliation200ResponseDataModelStateState**](AffiliationsGetOrganisationAffiliation200ResponseDataModelStateState.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.affiliations_get_organisation_affiliation200_response_data_model_state import AffiliationsGetOrganisationAffiliation200ResponseDataModelState

# TODO update the JSON string below
json = "{}"
# create an instance of AffiliationsGetOrganisationAffiliation200ResponseDataModelState from a JSON string
affiliations_get_organisation_affiliation200_response_data_model_state_instance = AffiliationsGetOrganisationAffiliation200ResponseDataModelState.from_json(json)
# print the JSON string representation of the object
print(AffiliationsGetOrganisationAffiliation200ResponseDataModelState.to_json())

# convert the object into a dict
affiliations_get_organisation_affiliation200_response_data_model_state_dict = affiliations_get_organisation_affiliation200_response_data_model_state_instance.to_dict()
# create an instance of AffiliationsGetOrganisationAffiliation200ResponseDataModelState from a dict
affiliations_get_organisation_affiliation200_response_data_model_state_from_dict = AffiliationsGetOrganisationAffiliation200ResponseDataModelState.from_dict(affiliations_get_organisation_affiliation200_response_data_model_state_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


