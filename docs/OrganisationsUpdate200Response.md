# OrganisationsUpdate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Organisation**](Organisation.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisations_update200_response import OrganisationsUpdate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationsUpdate200Response from a JSON string
organisations_update200_response_instance = OrganisationsUpdate200Response.from_json(json)
# print the JSON string representation of the object
print(OrganisationsUpdate200Response.to_json())

# convert the object into a dict
organisations_update200_response_dict = organisations_update200_response_instance.to_dict()
# create an instance of OrganisationsUpdate200Response from a dict
organisations_update200_response_from_dict = OrganisationsUpdate200Response.from_dict(organisations_update200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


