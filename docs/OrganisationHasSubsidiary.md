# OrganisationHasSubsidiary

Pivot model representing the relationship between organisations and subsidiaries

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**organisation_id** | **int** | ID of the organisation | [optional] 
**subsidiary_id** | **int** | ID of the subsidiary | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisation_has_subsidiary import OrganisationHasSubsidiary

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationHasSubsidiary from a JSON string
organisation_has_subsidiary_instance = OrganisationHasSubsidiary.from_json(json)
# print the JSON string representation of the object
print(OrganisationHasSubsidiary.to_json())

# convert the object into a dict
organisation_has_subsidiary_dict = organisation_has_subsidiary_instance.to_dict()
# create an instance of OrganisationHasSubsidiary from a dict
organisation_has_subsidiary_from_dict = OrganisationHasSubsidiary.from_dict(organisation_has_subsidiary_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


