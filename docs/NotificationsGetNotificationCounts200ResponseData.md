# NotificationsGetNotificationCounts200ResponseData


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**total** | **int** |  | [optional] 
**read** | **int** |  | [optional] 
**unread** | **int** |  | [optional] 

## Example

```python
from safepeopleregistry_api_sdk.models.notifications_get_notification_counts200_response_data import NotificationsGetNotificationCounts200ResponseData

# TODO update the JSON string below
json = "{}"
# create an instance of NotificationsGetNotificationCounts200ResponseData from a JSON string
notifications_get_notification_counts200_response_data_instance = NotificationsGetNotificationCounts200ResponseData.from_json(json)
# print the JSON string representation of the object
print(NotificationsGetNotificationCounts200ResponseData.to_json())

# convert the object into a dict
notifications_get_notification_counts200_response_data_dict = notifications_get_notification_counts200_response_data_instance.to_dict()
# create an instance of NotificationsGetNotificationCounts200ResponseData from a dict
notifications_get_notification_counts200_response_data_from_dict = NotificationsGetNotificationCounts200ResponseData.from_dict(notifications_get_notification_counts200_response_data_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


