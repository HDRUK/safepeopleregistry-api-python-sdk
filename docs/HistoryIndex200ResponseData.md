# HistoryIndex200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] 
**created_at** | **str** |  | [optional] 
**updated_at** | **str** |  | [optional] 
**endorsement_id** | **int** |  | [optional] 
**infringement_id** | **int** |  | [optional] 
**project_id** | **int** |  | [optional] 
**access_key_id** | **int** |  | [optional] 
**custodian_identifier** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.history_index200_response_data import HistoryIndex200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of HistoryIndex200ResponseData from a JSON string
history_index200_response_data_instance = HistoryIndex200ResponseData.from_json(json)
# print the JSON string representation of the object
print(HistoryIndex200ResponseData.to_json())

# convert the object into a dict
history_index200_response_data_dict = history_index200_response_data_instance.to_dict()
# create an instance of HistoryIndex200ResponseData from a dict
history_index200_response_data_from_dict = HistoryIndex200ResponseData.from_dict(history_index200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


