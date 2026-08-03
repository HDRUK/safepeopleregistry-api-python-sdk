# HistoryStore201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**HistoryIndex200ResponseData**](HistoryIndex200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.history_store201_response import HistoryStore201Response

# TODO update the JSON string below
json = "{}"
# create an instance of HistoryStore201Response from a JSON string
history_store201_response_instance = HistoryStore201Response.from_json(json)
# print the JSON string representation of the object
print(HistoryStore201Response.to_json())

# convert the object into a dict
history_store201_response_dict = history_store201_response_instance.to_dict()
# create an instance of HistoryStore201Response from a dict
history_store201_response_from_dict = HistoryStore201Response.from_dict(history_store201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


