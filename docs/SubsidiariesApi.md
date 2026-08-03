# safepeopleregistry_api_sdk.SubsidiariesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**subsidiaries_destroy**](SubsidiariesApi.md#subsidiaries_destroy) | **DELETE** /api/v1/subsidiaries/{subsidiaryId}/organisations/{organisationId} | subsidiaries@destroy
[**subsidiaries_store**](SubsidiariesApi.md#subsidiaries_store) | **POST** /api/v1/subsidiaries/organisations/{organisationId} | subsidiaries@store
[**subsidiaries_update**](SubsidiariesApi.md#subsidiaries_update) | **PUT** /api/v1/subsidiaries/{subsidiaryId}/organisations/{organisationId} | subsidiaries@update


# **subsidiaries_destroy**
> AffiliationDestroy200Response subsidiaries_destroy(organisation_id, subsidiary_id)

subsidiaries@destroy

Delete an subsidiary entry from the system

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
    api_instance = safepeopleregistry_api_sdk.SubsidiariesApi(api_client)
    organisation_id = 1 # int | organisations entry ID
    subsidiary_id = 1 # int | subsidiary entry ID

    try:
        # subsidiaries@destroy
        api_response = api_instance.subsidiaries_destroy(organisation_id, subsidiary_id)
        print("The response of SubsidiariesApi->subsidiaries_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubsidiariesApi->subsidiaries_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organisation_id** | **int**| organisations entry ID | 
 **subsidiary_id** | **int**| subsidiary entry ID | 

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

# **subsidiaries_store**
> SubsidiariesStore201Response subsidiaries_store(organisation_id, subsidiary)

subsidiaries@store

Create a subsidiary entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.subsidiaries_store201_response import SubsidiariesStore201Response
from safepeopleregistry_api_sdk.models.subsidiary import Subsidiary
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
    api_instance = safepeopleregistry_api_sdk.SubsidiariesApi(api_client)
    organisation_id = 1 # int | organisations entry ID
    subsidiary = safepeopleregistry_api_sdk.Subsidiary() # Subsidiary | subsidiary definition

    try:
        # subsidiaries@store
        api_response = api_instance.subsidiaries_store(organisation_id, subsidiary)
        print("The response of SubsidiariesApi->subsidiaries_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubsidiariesApi->subsidiaries_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organisation_id** | **int**| organisations entry ID | 
 **subsidiary** | [**Subsidiary**](Subsidiary.md)| subsidiary definition | 

### Return type

[**SubsidiariesStore201Response**](SubsidiariesStore201Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Success |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Not found response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **subsidiaries_update**
> SubsidiariesStore201Response subsidiaries_update(organisation_id, subsidiary_id, subsidiary)

subsidiaries@update

Update a subsidiary entry

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.subsidiaries_store201_response import SubsidiariesStore201Response
from safepeopleregistry_api_sdk.models.subsidiary import Subsidiary
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
    api_instance = safepeopleregistry_api_sdk.SubsidiariesApi(api_client)
    organisation_id = 1 # int | organisations entry ID
    subsidiary_id = 1 # int | subsidiary entry ID
    subsidiary = safepeopleregistry_api_sdk.Subsidiary() # Subsidiary | subsidiary definition

    try:
        # subsidiaries@update
        api_response = api_instance.subsidiaries_update(organisation_id, subsidiary_id, subsidiary)
        print("The response of SubsidiariesApi->subsidiaries_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SubsidiariesApi->subsidiaries_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organisation_id** | **int**| organisations entry ID | 
 **subsidiary_id** | **int**| subsidiary entry ID | 
 **subsidiary** | [**Subsidiary**](Subsidiary.md)| subsidiary definition | 

### Return type

[**SubsidiariesStore201Response**](SubsidiariesStore201Response.md)

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
**404** | Not found response |  -  |
**500** | Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

