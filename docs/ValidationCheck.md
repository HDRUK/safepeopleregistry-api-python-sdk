# ValidationCheck

Model representing validation checks

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the validation check | [optional] 
**name** | **str** | Name of the validation check | 
**description** | **str** | Description of the validation check | 
**applies_to** | **str** | Context to which the validation check applies | 
**enabled** | **bool** | Indicates whether the validation check is enabled | [optional] 
**created_at** | **datetime** | Timestamp when the validation check was created | [optional] 
**updated_at** | **datetime** | Timestamp when the validation check was last updated | [optional] 
**custodian_id** | **int** | Custodian id or null | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.validation_check import ValidationCheck

# TODO update the JSON string below
json = "{}"
# create an instance of ValidationCheck from a JSON string
validation_check_instance = ValidationCheck.from_json(json)
# print the JSON string representation of the object
print(ValidationCheck.to_json())

# convert the object into a dict
validation_check_dict = validation_check_instance.to_dict()
# create an instance of ValidationCheck from a dict
validation_check_from_dict = ValidationCheck.from_dict(validation_check_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


