# PendingInvitesIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**PendingInvite**](PendingInvite.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.pending_invites_index200_response import PendingInvitesIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of PendingInvitesIndex200Response from a JSON string
pending_invites_index200_response_instance = PendingInvitesIndex200Response.from_json(json)
# print the JSON string representation of the object
print(PendingInvitesIndex200Response.to_json())

# convert the object into a dict
pending_invites_index200_response_dict = pending_invites_index200_response_instance.to_dict()
# create an instance of PendingInvitesIndex200Response from a dict
pending_invites_index200_response_from_dict = PendingInvitesIndex200Response.from_dict(pending_invites_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


