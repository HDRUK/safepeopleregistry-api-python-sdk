# Affiliation

Affiliation model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**organisation_id** | **int** | Organisational link | [optional] 
**member_id** | **str** | Member ID UUID | [optional] 
**relationship** | **str** | Textual representation of affiliation relationship | [optional] 
**var_from** | **str** | Date affiliation commenced | [optional] 
**to** | **str** | Date affiliation concluded | [optional] 
**department** | **str** | Department worked during affiliation | [optional] 
**role** | **str** | Role held during affiliation | [optional] 
**email** | **str** | Professional email held during affiliation | [optional] 
**ror** | **str** | The ROR.org identifier for this affiliation institute | [optional] 
**registry_id** | **int** | The Registry primary key associated with this affiliation | [optional] 
**current_employer** | **bool** | Flag indicating if affiliation is for the current employer | [optional] 
**verification_code** | **str** | Unique verification code issued for confirmation | [optional] 
**verification_sent_at** | **datetime** | Timestamp when verification code was sent | [optional] 
**verification_confirmed_at** | **datetime** | Timestamp when verification was confirmed | [optional] 
**is_verified** | **bool** | Flag indicating if affiliation is verified | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.affiliation import Affiliation

# TODO update the JSON string below
json = "{}"
# create an instance of Affiliation from a JSON string
affiliation_instance = Affiliation.from_json(json)
# print the JSON string representation of the object
print(Affiliation.to_json())

# convert the object into a dict
affiliation_dict = affiliation_instance.to_dict()
# create an instance of Affiliation from a dict
affiliation_from_dict = Affiliation.from_dict(affiliation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


