# ValidationLogComment

Comments on validation logs

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**validation_log_id** | **int** | ID of the associated validation log | [optional] 
**user_id** | **int** | ID of the user who made the comment | [optional] 
**comment** | **str** | The comment text | [optional] 
**created_at** | **datetime** | Timestamp when the comment was created | [optional] 
**updated_at** | **datetime** | Timestamp when the comment was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.validation_log_comment import ValidationLogComment

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationLogComment from a JSON string
validation_log_comment_instance = ValidationLogComment.from_json(json)
# print the JSON string representation of the object
print(ValidationLogComment.to_json())

# convert the object into a dict
validation_log_comment_dict = validation_log_comment_instance.to_dict()
# create an instance of ValidationLogComment from a dict
validation_log_comment_from_dict = ValidationLogComment.from_dict(validation_log_comment_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


