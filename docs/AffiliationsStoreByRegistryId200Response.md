# AffiliationsStoreByRegistryId200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Affiliation**](Affiliation.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.affiliations_store_by_registry_id200_response import AffiliationsStoreByRegistryId200Response

# TODO update the JSON string below
json = "{}"
# create an instance of AffiliationsStoreByRegistryId200Response from a JSON string
affiliations_store_by_registry_id200_response_instance = AffiliationsStoreByRegistryId200Response.from_json(json)
# print the JSON string representation of the object
print(AffiliationsStoreByRegistryId200Response.to_json())

# convert the object into a dict
affiliations_store_by_registry_id200_response_dict = affiliations_store_by_registry_id200_response_instance.to_dict()
# create an instance of AffiliationsStoreByRegistryId200Response from a dict
affiliations_store_by_registry_id200_response_from_dict = AffiliationsStoreByRegistryId200Response.from_dict(affiliations_store_by_registry_id200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


