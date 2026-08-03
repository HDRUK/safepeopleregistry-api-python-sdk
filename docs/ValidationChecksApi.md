# safepeopleregistry_api_sdk.ValidationChecksApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**validation_checks_destroy**](ValidationChecksApi.md#validation_checks_destroy) | **DELETE** /api/v1/validation_checks/{id} | Delete a validation check
[**validation_checks_index**](ValidationChecksApi.md#validation_checks_index) | **GET** /api/v1/validation_checks | List all validation checks
[**validation_checks_show**](ValidationChecksApi.md#validation_checks_show) | **GET** /api/v1/validation_checks/{id} | Get a single validation check
[**validation_checks_store**](ValidationChecksApi.md#validation_checks_store) | **POST** /api/v1/validation_checks | Create a new validation check
[**validation_checks_update**](ValidationChecksApi.md#validation_checks_update) | **PUT** /api/v1/validation_checks/{id} | Update a validation check


# **validation_checks_destroy**
> ValidationChecksDestroy200Response validation_checks_destroy(id)

Delete a validation check

Remove a validation check.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_checks_destroy200_response import ValidationChecksDestroy200Response
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
    api_instance = safepeopleregistry_api_sdk.ValidationChecksApi(api_client)
    id = 56 # int | ID of the validation check

    try:
        # Delete a validation check
        api_response = api_instance.validation_checks_destroy(id)
        print("The response of ValidationChecksApi->validation_checks_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationChecksApi->validation_checks_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the validation check | 

### Return type

[**ValidationChecksDestroy200Response**](ValidationChecksDestroy200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Validation check deleted successfully |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Validation check not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validation_checks_index**
> List[ValidationCheck] validation_checks_index()

List all validation checks

Retrieve all validation checks.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_check import ValidationCheck
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
    api_instance = safepeopleregistry_api_sdk.ValidationChecksApi(api_client)

    try:
        # List all validation checks
        api_response = api_instance.validation_checks_index()
        print("The response of ValidationChecksApi->validation_checks_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationChecksApi->validation_checks_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[ValidationCheck]**](ValidationCheck.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Validation checks retrieved successfully |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validation_checks_show**
> ValidationCheck validation_checks_show(id)

Get a single validation check

Retrieve a specific validation check by ID.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_check import ValidationCheck
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
    api_instance = safepeopleregistry_api_sdk.ValidationChecksApi(api_client)
    id = 56 # int | ID of the validation check

    try:
        # Get a single validation check
        api_response = api_instance.validation_checks_show(id)
        print("The response of ValidationChecksApi->validation_checks_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationChecksApi->validation_checks_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the validation check | 

### Return type

[**ValidationCheck**](ValidationCheck.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Validation check retrieved successfully |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Validation check not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validation_checks_store**
> ValidationCheck validation_checks_store(validation_checks_store_request)

Create a new validation check

Create a new validation check entry.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_check import ValidationCheck
from safepeopleregistry_api_sdk.models.validation_checks_store_request import ValidationChecksStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.ValidationChecksApi(api_client)
    validation_checks_store_request = safepeopleregistry_api_sdk.ValidationChecksStoreRequest() # ValidationChecksStoreRequest | 

    try:
        # Create a new validation check
        api_response = api_instance.validation_checks_store(validation_checks_store_request)
        print("The response of ValidationChecksApi->validation_checks_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationChecksApi->validation_checks_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **validation_checks_store_request** | [**ValidationChecksStoreRequest**](ValidationChecksStoreRequest.md)|  | 

### Return type

[**ValidationCheck**](ValidationCheck.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Validation check created successfully |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **validation_checks_update**
> ValidationCheck validation_checks_update(id, validation_checks_store_request)

Update a validation check

Edit an existing validation check.

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.validation_check import ValidationCheck
from safepeopleregistry_api_sdk.models.validation_checks_store_request import ValidationChecksStoreRequest
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
    api_instance = safepeopleregistry_api_sdk.ValidationChecksApi(api_client)
    id = 56 # int | ID of the validation check
    validation_checks_store_request = safepeopleregistry_api_sdk.ValidationChecksStoreRequest() # ValidationChecksStoreRequest | 

    try:
        # Update a validation check
        api_response = api_instance.validation_checks_update(id, validation_checks_store_request)
        print("The response of ValidationChecksApi->validation_checks_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ValidationChecksApi->validation_checks_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the validation check | 
 **validation_checks_store_request** | [**ValidationChecksStoreRequest**](ValidationChecksStoreRequest.md)|  | 

### Return type

[**ValidationCheck**](ValidationCheck.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Validation check updated successfully |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Validation check not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

