# Experience

Model representing experiences

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the experience | [optional] 
**project_id** | **int** | ID of the project associated with the experience | [optional] 
**var_from** | **date** | Start date of the experience | [optional] 
**to** | **date** | End date of the experience | [optional] 
**organisation_id** | **int** | ID of the organisation associated with the experience | [optional] 
**created_at** | **datetime** | Timestamp when the experience was created | [optional] 
**updated_at** | **datetime** | Timestamp when the experience was last updated | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.experience import Experience

# TODO update the JSON string below
json = "{}"
# create an instance of Experience from a JSON string
experience_instance = Experience.from_json(json)
# print the JSON string representation of the object
print(Experience.to_json())

# convert the object into a dict
experience_dict = experience_instance.to_dict()
# create an instance of Experience from a dict
experience_from_dict = Experience.from_dict(experience_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


