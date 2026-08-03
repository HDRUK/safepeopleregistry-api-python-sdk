# safepeopleregistry_api_sdk.TrainingApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**training_index**](TrainingApi.md#training_index) | **GET** /api/v1/training | Training@index
[**training_index_by_registry_id**](TrainingApi.md#training_index_by_registry_id) | **GET** /api/v1/training/registry/{id} | Training@show
[**training_show**](TrainingApi.md#training_show) | **GET** /api/v1/training/{id} | Training@show
[**training_store**](TrainingApi.md#training_store) | **POST** /api/v1/training | Training@store
[**training_update**](TrainingApi.md#training_update) | **PUT** /api/v1/training/{id} | Training@update


# **training_index**
> TrainingShow200Response training_index()

Training@index

Return a list of Training entries

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.training_show200_response import TrainingShow200Response
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
    api_instance = safepeopleregistry_api_sdk.TrainingApi(api_client)

    try:
        # Training@index
        api_response = api_instance.training_index()
        print("The response of TrainingApi->training_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TrainingApi->training_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**TrainingShow200Response**](TrainingShow200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **training_index_by_registry_id**
> TrainingShow200Response training_index_by_registry_id(id)

Training@show

Return a list of training by registry id

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.training_show200_response import TrainingShow200Response
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
    api_instance = safepeopleregistry_api_sdk.TrainingApi(api_client)
    id = 1 # int | Training registry id

    try:
        # Training@show
        api_response = api_instance.training_index_by_registry_id(id)
        print("The response of TrainingApi->training_index_by_registry_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TrainingApi->training_index_by_registry_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Training registry id | 

### Return type

[**TrainingShow200Response**](TrainingShow200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **training_show**
> TrainingShow200Response training_show(id)

Training@show

Return a training record by registry id

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.training_show200_response import TrainingShow200Response
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
    api_instance = safepeopleregistry_api_sdk.TrainingApi(api_client)
    id = 1 # int | Training id

    try:
        # Training@show
        api_response = api_instance.training_show(id)
        print("The response of TrainingApi->training_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TrainingApi->training_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Training id | 

### Return type

[**TrainingShow200Response**](TrainingShow200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Not found response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **training_store**
> AccreditationStoreByRegistryId201Response training_store(training)

Training@store

Create a Training entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.training import Training
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
    api_instance = safepeopleregistry_api_sdk.TrainingApi(api_client)
    training = safepeopleregistry_api_sdk.Training() # Training | Training definition

    try:
        # Training@store
        api_response = api_instance.training_store(training)
        print("The response of TrainingApi->training_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TrainingApi->training_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **training** | [**Training**](Training.md)| Training definition | 

### Return type

[**AccreditationStoreByRegistryId201Response**](AccreditationStoreByRegistryId201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**201** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **training_update**
> TrainingUpdate200Response training_update(id, training)

Training@update

Update a Training entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.training import Training
from safepeopleregistry_api_sdk.models.training_update200_response import TrainingUpdate200Response
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
    api_instance = safepeopleregistry_api_sdk.TrainingApi(api_client)
    id = 1 # int | Training entry ID
    training = safepeopleregistry_api_sdk.Training() # Training | Training definition

    try:
        # Training@update
        api_response = api_instance.training_update(id, training)
        print("The response of TrainingApi->training_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling TrainingApi->training_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Training entry ID | 
 **training** | [**Training**](Training.md)| Training definition | 

### Return type

[**TrainingUpdate200Response**](TrainingUpdate200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**400** | Invalid argument(s) |  -  |
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

