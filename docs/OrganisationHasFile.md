# OrganisationHasFile

Pivot model representing the relationship between organisations and files

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**organisation_id** | **int** | ID of the organisation | [optional] 
**file_id** | **int** | ID of the file | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisation_has_file import OrganisationHasFile

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationHasFile from a JSON string
organisation_has_file_instance = OrganisationHasFile.from_json(json)
# print the JSON string representation of the object
print(OrganisationHasFile.to_json())

# convert the object into a dict
organisation_has_file_dict = organisation_has_file_instance.to_dict()
# create an instance of OrganisationHasFile from a dict
organisation_has_file_from_dict = OrganisationHasFile.from_dict(organisation_has_file_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


