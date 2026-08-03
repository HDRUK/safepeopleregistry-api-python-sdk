# OrganisationsGetRegistries200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**OrganisationsGetRegistries200ResponseData**](OrganisationsGetRegistries200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisations_get_registries200_response import OrganisationsGetRegistries200Response

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationsGetRegistries200Response from a JSON string
organisations_get_registries200_response_instance = OrganisationsGetRegistries200Response.from_json(json)
# print the JSON string representation of the object
print(OrganisationsGetRegistries200Response.to_json())

# convert the object into a dict
organisations_get_registries200_response_dict = organisations_get_registries200_response_instance.to_dict()
# create an instance of OrganisationsGetRegistries200Response from a dict
organisations_get_registries200_response_from_dict = OrganisationsGetRegistries200Response.from_dict(organisations_get_registries200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


