# OrganisationGetDelegates200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**List[OrganisationGetDelegates200ResponseDataInner]**](OrganisationGetDelegates200ResponseDataInner.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisation_get_delegates200_response import OrganisationGetDelegates200Response

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationGetDelegates200Response from a JSON string
organisation_get_delegates200_response_instance = OrganisationGetDelegates200Response.from_json(json)
# print the JSON string representation of the object
print(OrganisationGetDelegates200Response.to_json())

# convert the object into a dict
organisation_get_delegates200_response_dict = organisation_get_delegates200_response_instance.to_dict()
# create an instance of OrganisationGetDelegates200Response from a dict
organisation_get_delegates200_response_from_dict = OrganisationGetDelegates200Response.from_dict(organisation_get_delegates200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


