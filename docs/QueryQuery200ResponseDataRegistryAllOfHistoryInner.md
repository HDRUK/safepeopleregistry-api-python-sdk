# QueryQuery200ResponseDataRegistryAllOfHistoryInner


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
**affiliation** | [**Affiliation**](Affiliation.md) |  | [optional] 
**project** | [**Project**](Project.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.query_query200_response_data_registry_all_of_history_inner import QueryQuery200ResponseDataRegistryAllOfHistoryInner

# TODO update the JSON string below
json = "{}"
# create an instance of QueryQuery200ResponseDataRegistryAllOfHistoryInner from a JSON string
query_query200_response_data_registry_all_of_history_inner_instance = QueryQuery200ResponseDataRegistryAllOfHistoryInner.from_json(json)
# print the JSON string representation of the object
print(QueryQuery200ResponseDataRegistryAllOfHistoryInner.to_json())

# convert the object into a dict
query_query200_response_data_registry_all_of_history_inner_dict = query_query200_response_data_registry_all_of_history_inner_instance.to_dict()
# create an instance of QueryQuery200ResponseDataRegistryAllOfHistoryInner from a dict
query_query200_response_data_registry_all_of_history_inner_from_dict = QueryQuery200ResponseDataRegistryAllOfHistoryInner.from_dict(query_query200_response_data_registry_all_of_history_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


