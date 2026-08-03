# PendingInvite

Model representing pending invites

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the pending invite | [optional] 
**user_id** | **int** | ID of the user associated with the invite | [optional] 
**organisation_id** | **int** | ID of the organisation associated with the invite | [optional] 
**status** | **str** | Status of the invite | [optional] 
**invite_accepted_at** | **datetime** | Timestamp when the invite was accepted | [optional] 
**invite_sent_at** | **datetime** | Timestamp when the invite was sent | [optional] 
**invite_code** | **str** | Unique code for the invite | [optional] 
**created_at** | **datetime** | Timestamp when the invite record was created | [optional] 
**updated_at** | **datetime** | Timestamp when the invite record was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.pending_invite import PendingInvite

# TODO update the JSON string below
json = "{}"
# create an instance of PendingInvite from a JSON string
pending_invite_instance = PendingInvite.from_json(json)
# print the JSON string representation of the object
print(PendingInvite.to_json())

# convert the object into a dict
pending_invite_dict = pending_invite_instance.to_dict()
# create an instance of PendingInvite from a dict
pending_invite_from_dict = PendingInvite.from_dict(pending_invite_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


