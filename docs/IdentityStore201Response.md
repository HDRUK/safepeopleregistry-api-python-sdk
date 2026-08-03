# IdentityStore201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**IdentityStore201ResponseData**](IdentityStore201ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.identity_store201_response import IdentityStore201Response

# TODO update the JSON string below
json = "{}"
# create an instance of IdentityStore201Response from a JSON string
identity_store201_response_instance = IdentityStore201Response.from_json(json)
# print the JSON string representation of the object
print(IdentityStore201Response.to_json())

# convert the object into a dict
identity_store201_response_dict = identity_store201_response_instance.to_dict()
# create an instance of IdentityStore201Response from a dict
identity_store201_response_from_dict = IdentityStore201Response.from_dict(identity_store201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


