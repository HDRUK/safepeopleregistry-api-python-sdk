# OrganisationHasCharity

Pivot model representing the relationship between organisations and charities

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique identifier for the organisation-charity relationship | [optional] 
**organisation_id** | **int** | ID of the organisation | [optional] 
**charity_id** | **int** | ID of the charity | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.organisation_has_charity import OrganisationHasCharity

# TODO update the JSON string below
json = "{}"
# create an instance of OrganisationHasCharity from a JSON string
organisation_has_charity_instance = OrganisationHasCharity.from_json(json)
# print the JSON string representation of the object
print(OrganisationHasCharity.to_json())

# convert the object into a dict
organisation_has_charity_dict = organisation_has_charity_instance.to_dict()
# create an instance of OrganisationHasCharity from a dict
organisation_has_charity_from_dict = OrganisationHasCharity.from_dict(organisation_has_charity_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


