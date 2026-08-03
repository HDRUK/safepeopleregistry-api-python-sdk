# HistoryIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**HistoryIndex200ResponseData**](HistoryIndex200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.history_index200_response import HistoryIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of HistoryIndex200Response from a JSON string
history_index200_response_instance = HistoryIndex200Response.from_json(json)
# print the JSON string representation of the object
print(HistoryIndex200Response.to_json())

# convert the object into a dict
history_index200_response_dict = history_index200_response_instance.to_dict()
# create an instance of HistoryIndex200Response from a dict
history_index200_response_from_dict = HistoryIndex200Response.from_dict(history_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


