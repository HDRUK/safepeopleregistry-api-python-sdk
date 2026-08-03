# History

Model representing historical records

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the history record | [optional] 
**affiliation_id** | **int** | ID of the affiliation associated with the history record | [optional] 
**endorsement_id** | **int** | ID of the endorsement associated with the history record | [optional] 
**infringement_id** | **int** | ID of the infringement associated with the history record | [optional] 
**project_id** | **int** | ID of the project associated with the history record | [optional] 
**access_key_id** | **int** | ID of the access key associated with the history record | [optional] 
**custodian_identifier** | **str** | Identifier for the custodian associated with the history record | [optional] 
**ledger_hash** | **str** | Hash of the ledger associated with the history record | [optional] 
**created_at** | **datetime** | Timestamp when the history record was created | [optional] 
**updated_at** | **datetime** | Timestamp when the history record was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.history import History

# TODO update the JSON string below
json = "{}"
# create an instance of History from a JSON string
history_instance = History.from_json(json)
# print the JSON string representation of the object
print(History.to_json())

# convert the object into a dict
history_dict = history_instance.to_dict()
# create an instance of History from a dict
history_from_dict = History.from_dict(history_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


