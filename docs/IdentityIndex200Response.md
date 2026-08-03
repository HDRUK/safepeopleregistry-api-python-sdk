# IdentityIndex200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**IdentityIndex200ResponseData**](IdentityIndex200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.identity_index200_response import IdentityIndex200Response

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityIndex200Response from a JSON string
identity_index200_response_instance = IdentityIndex200Response.from_json(json)
# print the JSON string representation of the object
print(IdentityIndex200Response.to_json())

# convert the object into a dict
identity_index200_response_dict = identity_index200_response_instance.to_dict()
# create an instance of IdentityIndex200Response from a dict
identity_index200_response_from_dict = IdentityIndex200Response.from_dict(identity_index200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


