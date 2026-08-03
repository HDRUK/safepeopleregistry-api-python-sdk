# QueryQuery200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**QueryQuery200ResponseData**](QueryQuery200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.query_query200_response import QueryQuery200Response

# TODO update the JSON string below
json = "{}"
# create an instance of QueryQuery200Response from a JSON string
query_query200_response_instance = QueryQuery200Response.from_json(json)
# print the JSON string representation of the object
print(QueryQuery200Response.to_json())

# convert the object into a dict
query_query200_response_dict = query_query200_response_instance.to_dict()
# create an instance of QueryQuery200Response from a dict
query_query200_response_from_dict = QueryQuery200Response.from_dict(query_query200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


