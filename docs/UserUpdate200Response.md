# UserUpdate200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**UserUpdate200ResponseData**](UserUpdate200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.user_update200_response import UserUpdate200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UserUpdate200Response from a JSON string
user_update200_response_instance = UserUpdate200Response.from_json(json)
# print the JSON string representation of the object
print(UserUpdate200Response.to_json())

# convert the object into a dict
user_update200_response_dict = user_update200_response_instance.to_dict()
# create an instance of UserUpdate200Response from a dict
user_update200_response_from_dict = UserUpdate200Response.from_dict(user_update200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


