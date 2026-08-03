# EndorsementIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Endorsement**](Endorsement.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.endorsement_index200_response import EndorsementIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of EndorsementIndex200Response from a JSON string
endorsement_index200_response_instance = EndorsementIndex200Response.from_json(json)
# print the JSON string representation of the object
print(EndorsementIndex200Response.to_json())

# convert the object into a dict
endorsement_index200_response_dict = endorsement_index200_response_instance.to_dict()
# create an instance of EndorsementIndex200Response from a dict
endorsement_index200_response_from_dict = EndorsementIndex200Response.from_dict(endorsement_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


