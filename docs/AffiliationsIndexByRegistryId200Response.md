# AffiliationsIndexByRegistryId200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[Affiliation]**](Affiliation.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.affiliations_index_by_registry_id200_response import AffiliationsIndexByRegistryId200Response

# TODO update the JSON string below
json = "{}"
# create an instance of AffiliationsIndexByRegistryId200Response from a JSON string
affiliations_index_by_registry_id200_response_instance = AffiliationsIndexByRegistryId200Response.from_json(json)
# print the JSON string representation of the object
print(AffiliationsIndexByRegistryId200Response.to_json())

# convert the object into a dict
affiliations_index_by_registry_id200_response_dict = affiliations_index_by_registry_id200_response_instance.to_dict()
# create an instance of AffiliationsIndexByRegistryId200Response from a dict
affiliations_index_by_registry_id200_response_from_dict = AffiliationsIndexByRegistryId200Response.from_dict(affiliations_index_by_registry_id200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


