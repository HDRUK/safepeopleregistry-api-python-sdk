# safepeopleregistry_api_sdk.NotificationsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**notifications_get_notification_counts**](NotificationsApi.md#notifications_get_notification_counts) | **GET** /api/v1/users/{id}/notifications/count | Get notification counts for a specific user
[**notifications_get_user_notifications**](NotificationsApi.md#notifications_get_user_notifications) | **GET** /api/v1/users/{id}/notifications | Get notifications for a specific user
[**notifications_mark_user_notification_as_read**](NotificationsApi.md#notifications_mark_user_notification_as_read) | **PATCH** /api/v1/users/{id}/notifications/{notificationId}/read | Mark a specific notification as read
[**notifications_mark_user_notification_as_unread**](NotificationsApi.md#notifications_mark_user_notification_as_unread) | **PATCH** /api/v1/users/{id}/notifications/{notificationId}/unread | Mark a specific notification as unread
[**notifications_mark_user_notifications_as_read**](NotificationsApi.md#notifications_mark_user_notifications_as_read) | **PATCH** /api/v1/users/{id}/notifications/read | Mark all notifications as read for a specific user


# **notifications_get_notification_counts**
> NotificationsGetNotificationCounts200Response notifications_get_notification_counts(id)

Get notification counts for a specific user

Retrieve the total, read, and unread notification counts for a given user.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.notifications_get_notification_counts200_response import NotificationsGetNotificationCounts200Response
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.NotificationsApi(api_client)
    id = 56 # int | User ID

    try:
        # Get notification counts for a specific user
        api_response = api_instance.notifications_get_notification_counts(id)
        print("The response of NotificationsApi->notifications_get_notification_counts:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->notifications_get_notification_counts: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| User ID | 

### Return type

[**NotificationsGetNotificationCounts200Response**](NotificationsGetNotificationCounts200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |
**401** | Unauthorized |  -  |
**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **notifications_get_user_notifications**
> NotificationsGetUserNotifications200Response notifications_get_user_notifications(id, status=status)

Get notifications for a specific user

Retrieves notifications for a user, with an optional filter for read/unread notifications.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.notifications_get_user_notifications200_response import NotificationsGetUserNotifications200Response
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.NotificationsApi(api_client)
    id = 1 # int | User ID
    status = 'unread' # str | Filter notifications by status (read/unread) (optional)

    try:
        # Get notifications for a specific user
        api_response = api_instance.notifications_get_user_notifications(id, status=status)
        print("The response of NotificationsApi->notifications_get_user_notifications:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->notifications_get_user_notifications: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| User ID | 
 **status** | **str**| Filter notifications by status (read/unread) | [optional] 

### Return type

[**NotificationsGetUserNotifications200Response**](NotificationsGetUserNotifications200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful response |  -  |
**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **notifications_mark_user_notification_as_read**
> NotificationsMarkUserNotificationAsRead200Response notifications_mark_user_notification_as_read(id, notification_id)

Mark a specific notification as read

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.notifications_mark_user_notification_as_read200_response import NotificationsMarkUserNotificationAsRead200Response
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.NotificationsApi(api_client)
    id = 1 # int | User ID
    notification_id = 'abc95e84-0ebd-45d2-8129-9bf7ed043433' # str | Notification ID

    try:
        # Mark a specific notification as read
        api_response = api_instance.notifications_mark_user_notification_as_read(id, notification_id)
        print("The response of NotificationsApi->notifications_mark_user_notification_as_read:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->notifications_mark_user_notification_as_read: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| User ID | 
 **notification_id** | **str**| Notification ID | 

### Return type

[**NotificationsMarkUserNotificationAsRead200Response**](NotificationsMarkUserNotificationAsRead200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Notification marked as read |  -  |
**404** | User or notification not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **notifications_mark_user_notification_as_unread**
> notifications_mark_user_notification_as_unread(id, notification_id)

Mark a specific notification as unread

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.NotificationsApi(api_client)
    id = 1 # int | User ID
    notification_id = 'abc95e84-0ebd-45d2-8129-9bf7ed043433' # str | Notification ID

    try:
        # Mark a specific notification as unread
        api_instance.notifications_mark_user_notification_as_unread(id, notification_id)
    except Exception as e:
        print("Exception when calling NotificationsApi->notifications_mark_user_notification_as_unread: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| User ID | 
 **notification_id** | **str**| Notification ID | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Notification marked as unread |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **notifications_mark_user_notifications_as_read**
> NotificationsMarkUserNotificationsAsRead200Response notifications_mark_user_notifications_as_read(id)

Mark all notifications as read for a specific user

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.notifications_mark_user_notifications_as_read200_response import NotificationsMarkUserNotificationsAsRead200Response
from safepeopleregistry_api_sdk.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = safepeopleregistry_api_sdk.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with safepeopleregistry_api_sdk.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = safepeopleregistry_api_sdk.NotificationsApi(api_client)
    id = 1 # int | User ID

    try:
        # Mark all notifications as read for a specific user
        api_response = api_instance.notifications_mark_user_notifications_as_read(id)
        print("The response of NotificationsApi->notifications_mark_user_notifications_as_read:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->notifications_mark_user_notifications_as_read: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| User ID | 

### Return type

[**NotificationsMarkUserNotificationsAsRead200Response**](NotificationsMarkUserNotificationsAsRead200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Notifications marked as read |  -  |
**404** | User not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

