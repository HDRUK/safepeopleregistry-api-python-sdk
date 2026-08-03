# safepeopleregistry_api_sdk.WebhooksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**webhooks_create_receiver**](WebhooksApi.md#webhooks_create_receiver) | **POST** /api/v1/webhooks/receivers | Create a new webhook receiver
[**webhooks_delete_receiver**](WebhooksApi.md#webhooks_delete_receiver) | **DELETE** /api/v1/webhooks/receivers/{custodianId} | Delete a webhook receiver
[**webhooks_get_all_event_triggers**](WebhooksApi.md#webhooks_get_all_event_triggers) | **GET** /api/v1/webhooks/event-triggers | Get all webhook event triggers
[**webhooks_get_all_receivers**](WebhooksApi.md#webhooks_get_all_receivers) | **GET** /api/v1/webhooks/receivers | Get all webhook receivers
[**webhooks_get_receivers_by_custodian**](WebhooksApi.md#webhooks_get_receivers_by_custodian) | **GET** /api/v1/webhooks/receivers/{custodianId} | Get webhook receivers by custodian
[**webhooks_sendgrid**](WebhooksApi.md#webhooks_sendgrid) | **GET** /api/v1/webhooks/sendgrid | Get sendgrid webhook event triggers
[**webhooks_update_receiver**](WebhooksApi.md#webhooks_update_receiver) | **PUT** /api/v1/webhooks/receivers/{custodianId} | Update a webhook receiver


# **webhooks_create_receiver**
> WebhooksCreateReceiver201Response webhooks_create_receiver(webhooks_create_receiver_request)

Create a new webhook receiver

Creates a new webhook receiver for a custodian

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.webhooks_create_receiver201_response import WebhooksCreateReceiver201Response
from safepeopleregistry_api_sdk.models.webhooks_create_receiver_request import WebhooksCreateReceiverRequest
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
    api_instance = safepeopleregistry_api_sdk.WebhooksApi(api_client)
    webhooks_create_receiver_request = safepeopleregistry_api_sdk.WebhooksCreateReceiverRequest() # WebhooksCreateReceiverRequest | 

    try:
        # Create a new webhook receiver
        api_response = api_instance.webhooks_create_receiver(webhooks_create_receiver_request)
        print("The response of WebhooksApi->webhooks_create_receiver:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_create_receiver: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **webhooks_create_receiver_request** | [**WebhooksCreateReceiverRequest**](WebhooksCreateReceiverRequest.md)|  | 

### Return type

[**WebhooksCreateReceiver201Response**](WebhooksCreateReceiver201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful operation |  -  |
**422** | Validation error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooks_delete_receiver**
> EducationDestroyByRegistryId200Response webhooks_delete_receiver(custodian_id, webhooks_delete_receiver_request)

Delete a webhook receiver

Deletes a specific webhook receiver for a custodian

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.education_destroy_by_registry_id200_response import EducationDestroyByRegistryId200Response
from safepeopleregistry_api_sdk.models.webhooks_delete_receiver_request import WebhooksDeleteReceiverRequest
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
    api_instance = safepeopleregistry_api_sdk.WebhooksApi(api_client)
    custodian_id = 56 # int | 
    webhooks_delete_receiver_request = safepeopleregistry_api_sdk.WebhooksDeleteReceiverRequest() # WebhooksDeleteReceiverRequest | 

    try:
        # Delete a webhook receiver
        api_response = api_instance.webhooks_delete_receiver(custodian_id, webhooks_delete_receiver_request)
        print("The response of WebhooksApi->webhooks_delete_receiver:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_delete_receiver: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**|  | 
 **webhooks_delete_receiver_request** | [**WebhooksDeleteReceiverRequest**](WebhooksDeleteReceiverRequest.md)|  | 

### Return type

[**EducationDestroyByRegistryId200Response**](EducationDestroyByRegistryId200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Webhook receiver not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooks_get_all_event_triggers**
> WebhooksGetAllEventTriggers200Response webhooks_get_all_event_triggers()

Get all webhook event triggers

Returns all webhook event triggers

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.webhooks_get_all_event_triggers200_response import WebhooksGetAllEventTriggers200Response
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
    api_instance = safepeopleregistry_api_sdk.WebhooksApi(api_client)

    try:
        # Get all webhook event triggers
        api_response = api_instance.webhooks_get_all_event_triggers()
        print("The response of WebhooksApi->webhooks_get_all_event_triggers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_get_all_event_triggers: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**WebhooksGetAllEventTriggers200Response**](WebhooksGetAllEventTriggers200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooks_get_all_receivers**
> WebhooksGetAllReceivers200Response webhooks_get_all_receivers()

Get all webhook receivers

Returns all webhook receivers with their associated event trigger details

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.webhooks_get_all_receivers200_response import WebhooksGetAllReceivers200Response
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
    api_instance = safepeopleregistry_api_sdk.WebhooksApi(api_client)

    try:
        # Get all webhook receivers
        api_response = api_instance.webhooks_get_all_receivers()
        print("The response of WebhooksApi->webhooks_get_all_receivers:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_get_all_receivers: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**WebhooksGetAllReceivers200Response**](WebhooksGetAllReceivers200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooks_get_receivers_by_custodian**
> WebhooksGetAllReceivers200Response webhooks_get_receivers_by_custodian(custodian_id)

Get webhook receivers by custodian

Returns all webhook receivers for a specific custodian with their associated event trigger details

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.webhooks_get_all_receivers200_response import WebhooksGetAllReceivers200Response
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
    api_instance = safepeopleregistry_api_sdk.WebhooksApi(api_client)
    custodian_id = 56 # int | 

    try:
        # Get webhook receivers by custodian
        api_response = api_instance.webhooks_get_receivers_by_custodian(custodian_id)
        print("The response of WebhooksApi->webhooks_get_receivers_by_custodian:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_get_receivers_by_custodian: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**|  | 

### Return type

[**WebhooksGetAllReceivers200Response**](WebhooksGetAllReceivers200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |
**400** | Invalid argument(s) |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooks_sendgrid**
> webhooks_sendgrid()

Get sendgrid webhook event triggers

Returns sendgrid webhook event triggers

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
    api_instance = safepeopleregistry_api_sdk.WebhooksApi(api_client)

    try:
        # Get sendgrid webhook event triggers
        api_instance.webhooks_sendgrid()
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_sendgrid: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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
**200** | Successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **webhooks_update_receiver**
> EducationDestroyByRegistryId200Response webhooks_update_receiver(custodian_id, webhooks_update_receiver_request)

Update a webhook receiver

Updates a specific webhook receiver for a custodian

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.education_destroy_by_registry_id200_response import EducationDestroyByRegistryId200Response
from safepeopleregistry_api_sdk.models.webhooks_update_receiver_request import WebhooksUpdateReceiverRequest
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
    api_instance = safepeopleregistry_api_sdk.WebhooksApi(api_client)
    custodian_id = 56 # int | 
    webhooks_update_receiver_request = safepeopleregistry_api_sdk.WebhooksUpdateReceiverRequest() # WebhooksUpdateReceiverRequest | 

    try:
        # Update a webhook receiver
        api_response = api_instance.webhooks_update_receiver(custodian_id, webhooks_update_receiver_request)
        print("The response of WebhooksApi->webhooks_update_receiver:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling WebhooksApi->webhooks_update_receiver: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**|  | 
 **webhooks_update_receiver_request** | [**WebhooksUpdateReceiverRequest**](WebhooksUpdateReceiverRequest.md)|  | 

### Return type

[**EducationDestroyByRegistryId200Response**](EducationDestroyByRegistryId200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful operation |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Webhook receiver not found |  -  |
**422** | Validation error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

