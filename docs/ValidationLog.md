# ValidationLog

Validation Log model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Model primary key | [optional] 
**entity_type** | **str** | Type of the primary entity associated with the validation log | [optional] 
**entity_id** | **int** | ID of the primary entity associated with the validation log | [optional] 
**secondary_entity_type** | **str** | Type of the secondary entity associated with the validation log | [optional] 
**secondary_entity_id** | **int** | ID of the secondary entity associated with the validation log | [optional] 
**tertiary_entity_type** | **str** | Type of the tertiary entity associated with the validation log | [optional] 
**tertiary_entity_id** | **int** | ID of the tertiary entity associated with the validation log | [optional] 
**name** | **str** | Name of the validation log entry | [optional] 
**completed_at** | **datetime** | Timestamp when the validation was completed (nullable) | [optional] 
**manually_confirmed** | **bool** | Whether the validation was manually confirmed | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.validation_log import ValidationLog

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationLog from a JSON string
validation_log_instance = ValidationLog.from_json(json)
# print the JSON string representation of the object
print(ValidationLog.to_json())

# convert the object into a dict
validation_log_dict = validation_log_instance.to_dict()
# create an instance of ValidationLog from a dict
validation_log_from_dict = ValidationLog.from_dict(validation_log_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


