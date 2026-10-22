# OrganisationsInviteSro201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | **int** | ID of the invited user | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisations_invite_sro201_response import OrganisationsInviteSro201Response

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationsInviteSro201Response from a JSON string
organisations_invite_sro201_response_instance = OrganisationsInviteSro201Response.from_json(json)
# print the JSON string representation of the object
print(OrganisationsInviteSro201Response.to_json())

# convert the object into a dict
organisations_invite_sro201_response_dict = organisations_invite_sro201_response_instance.to_dict()
# create an instance of OrganisationsInviteSro201Response from a dict
organisations_invite_sro201_response_from_dict = OrganisationsInviteSro201Response.from_dict(organisations_invite_sro201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


