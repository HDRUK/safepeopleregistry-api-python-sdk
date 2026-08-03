# safepeopleregistry_api_sdk.CustodianModelConfigApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**custodian_model_config_destroy**](CustodianModelConfigApi.md#custodian_model_config_destroy) | **DELETE** /api/v1/custodian_config/{id} | CustodianModelConfig@destroy
[**custodian_model_config_get_by_custodian_id**](CustodianModelConfigApi.md#custodian_model_config_get_by_custodian_id) | **GET** /api/v1/custodian_config/{id} | CustodianModelConfig@getByCustodianID
[**custodian_model_config_get_entity_models**](CustodianModelConfigApi.md#custodian_model_config_get_entity_models) | **GET** /api/v1/custodian_config/{custodianId}/entity_models | Get entity models for custodian config
[**custodian_model_config_store**](CustodianModelConfigApi.md#custodian_model_config_store) | **POST** /api/v1/custodian_config | CustodianModelConfig@store
[**custodian_model_config_update**](CustodianModelConfigApi.md#custodian_model_config_update) | **PUT** /api/v1/custodian_config/{id} | CustodianModelConfig@update
[**custodian_model_config_update_entity_models**](CustodianModelConfigApi.md#custodian_model_config_update_entity_models) | **PUT** /api/v1/custodian_config/{custodianId}/entity_models | Update a custodian&#39;s entity models


# **custodian_model_config_destroy**
> AffiliationDestroy200Response custodian_model_config_destroy(id)

CustodianModelConfig@destroy

Delete a CustodianModelConfig entry from the system

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.affiliation_destroy200_response import AffiliationDestroy200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianModelConfigApi(api_client)
    id = 1 # int | CustodianModelConfig entry ID

    try:
        # CustodianModelConfig@destroy
        api_response = api_instance.custodian_model_config_destroy(id)
        print("The response of CustodianModelConfigApi->custodian_model_config_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianModelConfigApi->custodian_model_config_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| CustodianModelConfig entry ID | 

### Return type

[**AffiliationDestroy200Response**](AffiliationDestroy200Response.md)

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
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_model_config_get_by_custodian_id**
> CustodianModelConfigGetByCustodianID200Response custodian_model_config_get_by_custodian_id(id)

CustodianModelConfig@getByCustodianID

Return a list of Custodian config

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_model_config_get_by_custodian_id200_response import CustodianModelConfigGetByCustodianID200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianModelConfigApi(api_client)
    id = 1 # int | CustodianModelConfig entry ID

    try:
        # CustodianModelConfig@getByCustodianID
        api_response = api_instance.custodian_model_config_get_by_custodian_id(id)
        print("The response of CustodianModelConfigApi->custodian_model_config_get_by_custodian_id:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianModelConfigApi->custodian_model_config_get_by_custodian_id: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| CustodianModelConfig entry ID | 

### Return type

[**CustodianModelConfigGetByCustodianID200Response**](CustodianModelConfigGetByCustodianID200Response.md)

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

# **custodian_model_config_get_entity_models**
> CustodianModelConfigGetEntityModels200Response custodian_model_config_get_entity_models(custodian_id, entity_model_type)

Get entity models for custodian config

Retrieve entity models associated with custodian config based on the specified entity_model_type

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_model_config_get_entity_models200_response import CustodianModelConfigGetEntityModels200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianModelConfigApi(api_client)
    custodian_id = 56 # int | ID of the custodian
    entity_model_type = 'entity_model_type_example' # str | Type of entity model to retrieve

    try:
        # Get entity models for custodian config
        api_response = api_instance.custodian_model_config_get_entity_models(custodian_id, entity_model_type)
        print("The response of CustodianModelConfigApi->custodian_model_config_get_entity_models:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianModelConfigApi->custodian_model_config_get_entity_models: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 
 **entity_model_type** | **str**| Type of entity model to retrieve | 

### Return type

[**CustodianModelConfigGetEntityModels200Response**](CustodianModelConfigGetEntityModels200Response.md)

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

# **custodian_model_config_store**
> CustodianModelConfigUpdate200Response custodian_model_config_store(custodian_model_config)

CustodianModelConfig@store

Create a CustodianModelConfig entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_model_config import CustodianModelConfig
from safepeopleregistry_api_sdk.models.custodian_model_config_update200_response import CustodianModelConfigUpdate200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianModelConfigApi(api_client)
    custodian_model_config = safepeopleregistry_api_sdk.CustodianModelConfig() # CustodianModelConfig | CustodianModelConfig definition

    try:
        # CustodianModelConfig@store
        api_response = api_instance.custodian_model_config_store(custodian_model_config)
        print("The response of CustodianModelConfigApi->custodian_model_config_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianModelConfigApi->custodian_model_config_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_model_config** | [**CustodianModelConfig**](CustodianModelConfig.md)| CustodianModelConfig definition | 

### Return type

[**CustodianModelConfigUpdate200Response**](CustodianModelConfigUpdate200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**404** | Not found response |  -  |
**200** | Success |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **custodian_model_config_update**
> CustodianModelConfigUpdate200Response custodian_model_config_update(id, custodian_model_config)

CustodianModelConfig@update

Update an CustodianModelConfig entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_model_config import CustodianModelConfig
from safepeopleregistry_api_sdk.models.custodian_model_config_update200_response import CustodianModelConfigUpdate200Response
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
    api_instance = safepeopleregistry_api_sdk.CustodianModelConfigApi(api_client)
    id = 1 # int | CustodianModelConfig entry ID
    custodian_model_config = safepeopleregistry_api_sdk.CustodianModelConfig() # CustodianModelConfig | CustodianModelConfig definition

    try:
        # CustodianModelConfig@update
        api_response = api_instance.custodian_model_config_update(id, custodian_model_config)
        print("The response of CustodianModelConfigApi->custodian_model_config_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianModelConfigApi->custodian_model_config_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| CustodianModelConfig entry ID | 
 **custodian_model_config** | [**CustodianModelConfig**](CustodianModelConfig.md)| CustodianModelConfig definition | 

### Return type

[**CustodianModelConfigUpdate200Response**](CustodianModelConfigUpdate200Response.md)

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

# **custodian_model_config_update_entity_models**
> CustodianModelConfigUpdateEntityModels200Response custodian_model_config_update_entity_models(custodian_id, custodian_model_config_update_entity_models_request)

Update a custodian's entity models

Update the active status of specified custodian model configs for a given custodian

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.custodian_model_config_update_entity_models200_response import CustodianModelConfigUpdateEntityModels200Response
from safepeopleregistry_api_sdk.models.custodian_model_config_update_entity_models_request import CustodianModelConfigUpdateEntityModelsRequest
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
    api_instance = safepeopleregistry_api_sdk.CustodianModelConfigApi(api_client)
    custodian_id = 56 # int | ID of the custodian
    custodian_model_config_update_entity_models_request = safepeopleregistry_api_sdk.CustodianModelConfigUpdateEntityModelsRequest() # CustodianModelConfigUpdateEntityModelsRequest | 

    try:
        # Update a custodian's entity models
        api_response = api_instance.custodian_model_config_update_entity_models(custodian_id, custodian_model_config_update_entity_models_request)
        print("The response of CustodianModelConfigApi->custodian_model_config_update_entity_models:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CustodianModelConfigApi->custodian_model_config_update_entity_models: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **custodian_id** | **int**| ID of the custodian | 
 **custodian_model_config_update_entity_models_request** | [**CustodianModelConfigUpdateEntityModelsRequest**](CustodianModelConfigUpdateEntityModelsRequest.md)|  | 

### Return type

[**CustodianModelConfigUpdateEntityModels200Response**](CustodianModelConfigUpdateEntityModels200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Not Found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

