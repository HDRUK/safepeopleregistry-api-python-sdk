# Accreditation

Accreditation model

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the accreditation | [optional] 
**associated_organisation_name** | **str** | Name of the associated organisation | [optional] 
**id_string** | **str** | ID string for the accreditation | [optional] 
**issue_date** | **date** | Date when the accreditation was issued | [optional] 
**expiry_date** | **date** | Date when the accreditation expires | [optional] 
**created_at** | **datetime** | Timestamp when the accreditation was created | [optional] 
**updated_at** | **datetime** | Timestamp when the accreditation was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.accreditation import Accreditation

# TODO update the JSON string below
json = "{}"
# create an instance of Accreditation from a JSON string
accreditation_instance = Accreditation.from_json(json)
# print the JSON string representation of the object
print(Accreditation.to_json())

# convert the object into a dict
accreditation_dict = accreditation_instance.to_dict()
# create an instance of Accreditation from a dict
accreditation_from_dict = Accreditation.from_dict(accreditation_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


