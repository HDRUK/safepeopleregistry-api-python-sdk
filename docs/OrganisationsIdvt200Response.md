# OrganisationsIdvt200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**OrganisationsIdvt200ResponseData**](OrganisationsIdvt200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisations_idvt200_response import OrganisationsIdvt200Response

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationsIdvt200Response from a JSON string
organisations_idvt200_response_instance = OrganisationsIdvt200Response.from_json(json)
# print the JSON string representation of the object
print(OrganisationsIdvt200Response.to_json())

# convert the object into a dict
organisations_idvt200_response_dict = organisations_idvt200_response_instance.to_dict()
# create an instance of OrganisationsIdvt200Response from a dict
organisations_idvt200_response_from_dict = OrganisationsIdvt200Response.from_dict(organisations_idvt200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


