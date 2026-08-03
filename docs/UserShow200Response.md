# UserShow200Response


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | [optional] 
**data** | [**UserShow200ResponseData**](UserShow200ResponseData.md) |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.user_show200_response import UserShow200Response

# TODO update the JSON string below
json = "{}"
# create an instance of UserShow200Response from a JSON string
user_show200_response_instance = UserShow200Response.from_json(json)
# print the JSON string representation of the object
print(UserShow200Response.to_json())

# convert the object into a dict
user_show200_response_dict = user_show200_response_instance.to_dict()
# create an instance of UserShow200Response from a dict
user_show200_response_from_dict = UserShow200Response.from_dict(user_show200_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


