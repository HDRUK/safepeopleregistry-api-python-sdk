# HistoryStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**endorsement_id** | **int** |  | [optional] 
**infringement_id** | **int** |  | [optional] 
**project_id** | **int** |  | [optional] 
**access_key_id** | **int** |  | [optional] 
**custodian_identifier** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.history_store_request import HistoryStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of HistoryStoreRequest from a JSON string
history_store_request_instance = HistoryStoreRequest.from_json(json)
# print the JSON string representation of the object
print(HistoryStoreRequest.to_json())

# convert the object into a dict
history_store_request_dict = history_store_request_instance.to_dict()
# create an instance of HistoryStoreRequest from a dict
history_store_request_from_dict = HistoryStoreRequest.from_dict(history_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


