# ValidationLogCommentsUpdateRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**comment** | **str** | Updated comment text | 

## Example

```python
from safepeopleregistry_api_sdk.models.validation_log_comments_update_request import ValidationLogCommentsUpdateRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationLogCommentsUpdateRequest from a JSON string
validation_log_comments_update_request_instance = ValidationLogCommentsUpdateRequest.from_json(json)
# print the JSON string representation of the object
print(ValidationLogCommentsUpdateRequest.to_json())

# convert the object into a dict
validation_log_comments_update_request_dict = validation_log_comments_update_request_instance.to_dict()
# create an instance of ValidationLogCommentsUpdateRequest from a dict
validation_log_comments_update_request_from_dict = ValidationLogCommentsUpdateRequest.from_dict(validation_log_comments_update_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


