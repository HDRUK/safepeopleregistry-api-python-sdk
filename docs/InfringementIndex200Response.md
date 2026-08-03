# InfringementIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**Infringement**](Infringement.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.infringement_index200_response import InfringementIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of InfringementIndex200Response from a JSON string
infringement_index200_response_instance = InfringementIndex200Response.from_json(json)
# print the JSON string representation of the object
print(InfringementIndex200Response.to_json())

# convert the object into a dict
infringement_index200_response_dict = infringement_index200_response_instance.to_dict()
# create an instance of InfringementIndex200Response from a dict
infringement_index200_response_from_dict = InfringementIndex200Response.from_dict(infringement_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


