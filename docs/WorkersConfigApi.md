# autoppia_backend_client.WorkersConfigApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**workers_config_workers_create**](WorkersConfigApi.md#workers_config_workers_create) | **POST** /workers-config/workers/ | 
[**workers_config_workers_delete**](WorkersConfigApi.md#workers_config_workers_delete) | **DELETE** /workers-config/workers/{id}/ | 
[**workers_config_workers_deploy_info_list**](WorkersConfigApi.md#workers_config_workers_deploy_info_list) | **GET** /workers-config/workers/{id}/deploy-info/ | 
[**workers_config_workers_deploy_list**](WorkersConfigApi.md#workers_config_workers_deploy_list) | **GET** /workers-config/workers/{id}/deploy/ | 
[**workers_config_workers_deploy_stop_list**](WorkersConfigApi.md#workers_config_workers_deploy_stop_list) | **GET** /workers-config/workers/{id}/deploy-stop/ | 
[**workers_config_workers_list**](WorkersConfigApi.md#workers_config_workers_list) | **GET** /workers-config/workers/ | 
[**workers_config_workers_partial_update**](WorkersConfigApi.md#workers_config_workers_partial_update) | **PATCH** /workers-config/workers/{id}/ | 
[**workers_config_workers_read**](WorkersConfigApi.md#workers_config_workers_read) | **GET** /workers-config/workers/{id}/ | 
[**workers_config_workers_update**](WorkersConfigApi.md#workers_config_workers_update) | **PUT** /workers-config/workers/{id}/ | 


# **workers_config_workers_create**
> WorkerConfig workers_config_workers_create(data)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.WorkersConfigApi(api_client)
    data = autoppia_backend_client.WorkerConfig() # WorkerConfig | 

    try:
        api_response = api_instance.workers_config_workers_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling WorkersConfigApi->workers_config_workers_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**WorkerConfig**](WorkerConfig.md)|  | 

### Return type

[**WorkerConfig**](WorkerConfig.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **workers_config_workers_delete**
> workers_config_workers_delete(id)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.WorkersConfigApi(api_client)
    id = 56 # int | A unique integer value identifying this worker config.

    try:
        api_instance.workers_config_workers_delete(id)
    except ApiException as e:
        print("Exception when calling WorkersConfigApi->workers_config_workers_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker config. | 

### Return type

void (empty response body)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **workers_config_workers_deploy_info_list**
> list[WorkerConfig] workers_config_workers_deploy_info_list(id)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.WorkersConfigApi(api_client)
    id = 56 # int | A unique integer value identifying this worker config.

    try:
        api_response = api_instance.workers_config_workers_deploy_info_list(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling WorkersConfigApi->workers_config_workers_deploy_info_list: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker config. | 

### Return type

[**list[WorkerConfig]**](WorkerConfig.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **workers_config_workers_deploy_list**
> list[WorkerConfig] workers_config_workers_deploy_list(id)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.WorkersConfigApi(api_client)
    id = 56 # int | A unique integer value identifying this worker config.

    try:
        api_response = api_instance.workers_config_workers_deploy_list(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling WorkersConfigApi->workers_config_workers_deploy_list: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker config. | 

### Return type

[**list[WorkerConfig]**](WorkerConfig.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **workers_config_workers_deploy_stop_list**
> list[WorkerConfig] workers_config_workers_deploy_stop_list(id)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.WorkersConfigApi(api_client)
    id = 56 # int | A unique integer value identifying this worker config.

    try:
        api_response = api_instance.workers_config_workers_deploy_stop_list(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling WorkersConfigApi->workers_config_workers_deploy_stop_list: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker config. | 

### Return type

[**list[WorkerConfig]**](WorkerConfig.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **workers_config_workers_list**
> list[WorkerConfig] workers_config_workers_list()



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.WorkersConfigApi(api_client)
    
    try:
        api_response = api_instance.workers_config_workers_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling WorkersConfigApi->workers_config_workers_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[WorkerConfig]**](WorkerConfig.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **workers_config_workers_partial_update**
> WorkerConfig workers_config_workers_partial_update(id, data)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.WorkersConfigApi(api_client)
    id = 56 # int | A unique integer value identifying this worker config.
data = autoppia_backend_client.WorkerConfig() # WorkerConfig | 

    try:
        api_response = api_instance.workers_config_workers_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling WorkersConfigApi->workers_config_workers_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker config. | 
 **data** | [**WorkerConfig**](WorkerConfig.md)|  | 

### Return type

[**WorkerConfig**](WorkerConfig.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **workers_config_workers_read**
> WorkerConfig workers_config_workers_read(id)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.WorkersConfigApi(api_client)
    id = 56 # int | A unique integer value identifying this worker config.

    try:
        api_response = api_instance.workers_config_workers_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling WorkersConfigApi->workers_config_workers_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker config. | 

### Return type

[**WorkerConfig**](WorkerConfig.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **workers_config_workers_update**
> WorkerConfig workers_config_workers_update(id, data)



### Example

* Basic Authentication (Basic):
```python
from __future__ import print_function
import time
import autoppia_backend_client
from autoppia_backend_client.rest import ApiException
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = autoppia_backend_client.Configuration(
    host = "http://localhost"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure HTTP basic authorization: Basic
configuration = autoppia_backend_client.Configuration(
    username = 'YOUR_USERNAME',
    password = 'YOUR_PASSWORD'
)

# Enter a context with an instance of the API client
with autoppia_backend_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = autoppia_backend_client.WorkersConfigApi(api_client)
    id = 56 # int | A unique integer value identifying this worker config.
data = autoppia_backend_client.WorkerConfig() # WorkerConfig | 

    try:
        api_response = api_instance.workers_config_workers_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling WorkersConfigApi->workers_config_workers_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker config. | 
 **data** | [**WorkerConfig**](WorkerConfig.md)|  | 

### Return type

[**WorkerConfig**](WorkerConfig.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

