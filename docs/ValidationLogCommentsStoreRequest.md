# ValidationLogCommentsStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**validation_log_id** | **int** | ID of the associated validation log | 
**comment** | **str** | Comment text | 

## Example

```python
from safepeopleregistry_api_sdk.models.validation_log_comments_store_request import ValidationLogCommentsStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationLogCommentsStoreRequest from a JSON string
validation_log_comments_store_request_instance = ValidationLogCommentsStoreRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationLogCommentsStoreRequest.to_json())

# convert the object into a dict
validation_log_comments_store_request_dict = validation_log_comments_store_request_instance.to_dict()
# create an instance of ValidationLogCommentsStoreRequest from a dict
validation_log_comments_store_request_from_dict = ValidationLogCommentsStoreRequest.from_dict(validation_log_comments_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


