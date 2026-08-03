# safepeopleregistry_api_sdk.SectorApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sector_destroy**](SectorApi.md#sector_destroy) | **DELETE** /api/v1/sectors/{id} | Delete a sector
[**sector_index**](SectorApi.md#sector_index) | **GET** /api/v1/sectors | Get a list of sectors
[**sector_show**](SectorApi.md#sector_show) | **GET** /api/v1/sectors/{id} | Get a specific sector by ID
[**sector_store**](SectorApi.md#sector_store) | **POST** /api/v1/sectors | Create a new sector
[**sector_update**](SectorApi.md#sector_update) | **PUT** /api/v1/sectors/{id} | Update an existing sector


# **sector_destroy**
> AffiliationDestroy200Response sector_destroy(id)

Delete a sector

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
    api_instance = safepeopleregistry_api_sdk.SectorApi(api_client)
    id = 1 # int | ID of the sector

    try:
        # Delete a sector
        api_response = api_instance.sector_destroy(id)
        print("The response of SectorApi->sector_destroy:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SectorApi->sector_destroy: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the sector | 

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
**200** | Deleted |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Sector not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sector_index**
> List[Sector] sector_index()

Get a list of sectors

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.sector import Sector
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
    api_instance = safepeopleregistry_api_sdk.SectorApi(api_client)

    try:
        # Get a list of sectors
        api_response = api_instance.sector_index()
        print("The response of SectorApi->sector_index:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SectorApi->sector_index: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[Sector]**](Sector.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Success |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sector_show**
> Sector sector_show(id)

Get a specific sector by ID

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.sector import Sector
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
    api_instance = safepeopleregistry_api_sdk.SectorApi(api_client)
    id = 1 # int | ID of the sector

    try:
        # Get a specific sector by ID
        api_response = api_instance.sector_show(id)
        print("The response of SectorApi->sector_show:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SectorApi->sector_show: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the sector | 

### Return type

[**Sector**](Sector.md)

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
**404** | Sector not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sector_store**
> AccreditationStoreByRegistryId201Response sector_store(sector)

Create a new sector

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.accreditation_store_by_registry_id201_response import AccreditationStoreByRegistryId201Response
from safepeopleregistry_api_sdk.models.sector import Sector
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
    api_instance = safepeopleregistry_api_sdk.SectorApi(api_client)
    sector = safepeopleregistry_api_sdk.Sector() # Sector | 

    try:
        # Create a new sector
        api_response = api_instance.sector_store(sector)
        print("The response of SectorApi->sector_store:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SectorApi->sector_store: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sector** | [**Sector**](Sector.md)|  | 

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
**201** | Created |  -  |
**400** | Validation error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **sector_update**
> Sector sector_update(id, sector)

Update an existing sector

### Example


```python
import safepeopleregistry_api_sdk
from safepeopleregistry_api_sdk.models.sector import Sector
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
    api_instance = safepeopleregistry_api_sdk.SectorApi(api_client)
    id = 1 # int | ID of the sector
    sector = safepeopleregistry_api_sdk.Sector() # Sector | 

    try:
        # Update an existing sector
        api_response = api_instance.sector_update(id, sector)
        print("The response of SectorApi->sector_update:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SectorApi->sector_update: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| ID of the sector | 
 **sector** | [**Sector**](Sector.md)|  | 

### Return type

[**Sector**](Sector.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Updated |  -  |
**400** | Invalid argument(s) |  -  |
**404** | Sector not found |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

