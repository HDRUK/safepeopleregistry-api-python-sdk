# NotificationsGetUserNotifications200ResponseDataInner


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | [optional] 
**type** | **str** |  | [optional] 
**notifiable_type** | **str** |  | [optional] 
**notifiable_id** | **int** |  | [optional] 
**data** | [**NotificationsGetUserNotifications200ResponseDataInnerData**](NotificationsGetUserNotifications200ResponseDataInnerData.md) |  | [optional] 
**read_at** | **datetime** |  | [optional] 
**created_at** | **datetime** |  | [optional] 
**updated_at** | **datetime** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.notifications_get_user_notifications200_response_data_inner import NotificationsGetUserNotifications200ResponseDataInner

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationsGetUserNotifications200ResponseDataInner from a JSON string
notifications_get_user_notifications200_response_data_inner_instance = NotificationsGetUserNotifications200ResponseDataInner.from_json(json)
# print the JSON string representation of the object
print(NotificationsGetUserNotifications200ResponseDataInner.to_json())

# convert the object into a dict
notifications_get_user_notifications200_response_data_inner_dict = notifications_get_user_notifications200_response_data_inner_instance.to_dict()
# create an instance of NotificationsGetUserNotifications200ResponseDataInner from a dict
notifications_get_user_notifications200_response_data_inner_from_dict = NotificationsGetUserNotifications200ResponseDataInner.from_dict(notifications_get_user_notifications200_response_data_inner_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


