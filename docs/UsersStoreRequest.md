# UsersStoreRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**first_name** | **str** |  | [optional] 
**last_name** | **str** |  | [optional] 
**email** | **str** |  | [optional] 
**password** | **str** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.users_store_request import UsersStoreRequest

# TODO update the JSON string below
json = "{}"
# create an instance of UsersStoreRequest from a JSON string
users_store_request_instance = UsersStoreRequest.from_json(json)
# print the JSON string representation of the object
print(UsersStoreRequest.to_json())

# convert the object into a dict
users_store_request_dict = users_store_request_instance.to_dict()
# create an instance of UsersStoreRequest from a dict
users_store_request_from_dict = UsersStoreRequest.from_dict(users_store_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


