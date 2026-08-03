# Education

Model representing education records

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the education record | [optional] 
**title** | **str** | Title of the education qualification | [optional] 
**var_from** | **date** | Start date of the education qualification | [optional] 
**to** | **date** | End date of the education qualification | [optional] 
**institute_name** | **str** | Name of the educational institute | [optional] 
**institute_address** | **str** | Address of the educational institute | [optional] 
**institute_identifier** | **str** | Identifier for the educational institute | [optional] 
**source** | **str** | Source of the education record | [optional] 
**registry_id** | **int** | ID of the registry associated with the education record | [optional] 
**created_at** | **datetime** | Timestamp when the education record was created | [optional] 
**updated_at** | **datetime** | Timestamp when the education record was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.education import Education

# TODO update the JSON string below
json = "{}"
# create an instance of Education from a JSON string
education_instance = Education.from_json(json)
# print the JSON string representation of the object
print(Education.to_json())

# convert the object into a dict
education_dict = education_instance.to_dict()
# create an instance of Education from a dict
education_from_dict = Education.from_dict(education_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


