# QueryQueryRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ident** | **str** | The Registry&#39;s digi_ident value | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.query_query_request import QueryQueryRequest

# TODO update the JSON string below
json = "{}"
# create an instance of QueryQueryRequest from a JSON string
query_query_request_instance = QueryQueryRequest.from_json(json)
# print the JSON string representation of the object
print(QueryQueryRequest.to_json())

# convert the object into a dict
query_query_request_dict = query_query_request_instance.to_dict()
# create an instance of QueryQueryRequest from a dict
query_query_request_from_dict = QueryQueryRequest.from_dict(query_query_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


