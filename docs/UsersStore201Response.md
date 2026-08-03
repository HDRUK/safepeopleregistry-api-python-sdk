# UsersStore201Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**UsersStore201ResponseData**](UsersStore201ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.users_store201_response import UsersStore201Response

# TODO update the JSON string below
json = "{}"
# create an instance of UsersStore201Response from a JSON string
users_store201_response_instance = UsersStore201Response.from_json(json)
# print the JSON string representation of the object
print(UsersStore201Response.to_json())

# convert the object into a dict
users_store201_response_dict = users_store201_response_instance.to_dict()
# create an instance of UsersStore201Response from a dict
users_store201_response_from_dict = UsersStore201Response.from_dict(users_store201_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


