# autoppia_backend_client.ToolkitApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**toolkit_admin_toolkit_attribute_create**](ToolkitApi.md#toolkit_admin_toolkit_attribute_create) | **POST** /toolkit/admin/toolkit_attribute/ | 
[**toolkit_admin_toolkit_attribute_delete**](ToolkitApi.md#toolkit_admin_toolkit_attribute_delete) | **DELETE** /toolkit/admin/toolkit_attribute/{id}/ | 
[**toolkit_admin_toolkit_attribute_list**](ToolkitApi.md#toolkit_admin_toolkit_attribute_list) | **GET** /toolkit/admin/toolkit_attribute/ | 
[**toolkit_admin_toolkit_attribute_partial_update**](ToolkitApi.md#toolkit_admin_toolkit_attribute_partial_update) | **PATCH** /toolkit/admin/toolkit_attribute/{id}/ | 
[**toolkit_admin_toolkit_attribute_read**](ToolkitApi.md#toolkit_admin_toolkit_attribute_read) | **GET** /toolkit/admin/toolkit_attribute/{id}/ | 
[**toolkit_admin_toolkit_attribute_update**](ToolkitApi.md#toolkit_admin_toolkit_attribute_update) | **PUT** /toolkit/admin/toolkit_attribute/{id}/ | 
[**toolkit_admin_toolkit_create**](ToolkitApi.md#toolkit_admin_toolkit_create) | **POST** /toolkit/admin/toolkit/ | 
[**toolkit_admin_toolkit_delete**](ToolkitApi.md#toolkit_admin_toolkit_delete) | **DELETE** /toolkit/admin/toolkit/{id}/ | 
[**toolkit_admin_toolkit_linked_integration_create**](ToolkitApi.md#toolkit_admin_toolkit_linked_integration_create) | **POST** /toolkit/admin/toolkit_linked_integration/ | 
[**toolkit_admin_toolkit_linked_integration_delete**](ToolkitApi.md#toolkit_admin_toolkit_linked_integration_delete) | **DELETE** /toolkit/admin/toolkit_linked_integration/{id}/ | 
[**toolkit_admin_toolkit_linked_integration_list**](ToolkitApi.md#toolkit_admin_toolkit_linked_integration_list) | **GET** /toolkit/admin/toolkit_linked_integration/ | 
[**toolkit_admin_toolkit_linked_integration_partial_update**](ToolkitApi.md#toolkit_admin_toolkit_linked_integration_partial_update) | **PATCH** /toolkit/admin/toolkit_linked_integration/{id}/ | 
[**toolkit_admin_toolkit_linked_integration_read**](ToolkitApi.md#toolkit_admin_toolkit_linked_integration_read) | **GET** /toolkit/admin/toolkit_linked_integration/{id}/ | 
[**toolkit_admin_toolkit_linked_integration_update**](ToolkitApi.md#toolkit_admin_toolkit_linked_integration_update) | **PUT** /toolkit/admin/toolkit_linked_integration/{id}/ | 
[**toolkit_admin_toolkit_list**](ToolkitApi.md#toolkit_admin_toolkit_list) | **GET** /toolkit/admin/toolkit/ | 
[**toolkit_admin_toolkit_partial_update**](ToolkitApi.md#toolkit_admin_toolkit_partial_update) | **PATCH** /toolkit/admin/toolkit/{id}/ | 
[**toolkit_admin_toolkit_read**](ToolkitApi.md#toolkit_admin_toolkit_read) | **GET** /toolkit/admin/toolkit/{id}/ | 
[**toolkit_admin_toolkit_update**](ToolkitApi.md#toolkit_admin_toolkit_update) | **PUT** /toolkit/admin/toolkit/{id}/ | 
[**toolkit_tool_create**](ToolkitApi.md#toolkit_tool_create) | **POST** /toolkit/tool/ | 
[**toolkit_tool_delete**](ToolkitApi.md#toolkit_tool_delete) | **DELETE** /toolkit/tool/{id}/ | 
[**toolkit_tool_list**](ToolkitApi.md#toolkit_tool_list) | **GET** /toolkit/tool/ | 
[**toolkit_tool_partial_update**](ToolkitApi.md#toolkit_tool_partial_update) | **PATCH** /toolkit/tool/{id}/ | 
[**toolkit_tool_read**](ToolkitApi.md#toolkit_tool_read) | **GET** /toolkit/tool/{id}/ | 
[**toolkit_tool_update**](ToolkitApi.md#toolkit_tool_update) | **PUT** /toolkit/tool/{id}/ | 
[**toolkit_toolkit_list**](ToolkitApi.md#toolkit_toolkit_list) | **GET** /toolkit/toolkit/ | 
[**toolkit_toolkit_read**](ToolkitApi.md#toolkit_toolkit_read) | **GET** /toolkit/toolkit/{id}/ | 
[**toolkit_user_configuration_create**](ToolkitApi.md#toolkit_user_configuration_create) | **POST** /toolkit/user_configuration/ | 
[**toolkit_user_configuration_delete**](ToolkitApi.md#toolkit_user_configuration_delete) | **DELETE** /toolkit/user_configuration/{id}/ | 
[**toolkit_user_configuration_list**](ToolkitApi.md#toolkit_user_configuration_list) | **GET** /toolkit/user_configuration/ | 
[**toolkit_user_configuration_partial_update**](ToolkitApi.md#toolkit_user_configuration_partial_update) | **PATCH** /toolkit/user_configuration/{id}/ | 
[**toolkit_user_configuration_read**](ToolkitApi.md#toolkit_user_configuration_read) | **GET** /toolkit/user_configuration/{id}/ | 
[**toolkit_user_configuration_update**](ToolkitApi.md#toolkit_user_configuration_update) | **PUT** /toolkit/user_configuration/{id}/ | 
[**toolkit_user_toolkit_create**](ToolkitApi.md#toolkit_user_toolkit_create) | **POST** /toolkit/user_toolkit/ | 
[**toolkit_user_toolkit_delete**](ToolkitApi.md#toolkit_user_toolkit_delete) | **DELETE** /toolkit/user_toolkit/{id}/ | 
[**toolkit_user_toolkit_list**](ToolkitApi.md#toolkit_user_toolkit_list) | **GET** /toolkit/user_toolkit/ | 
[**toolkit_user_toolkit_partial_update**](ToolkitApi.md#toolkit_user_toolkit_partial_update) | **PATCH** /toolkit/user_toolkit/{id}/ | 
[**toolkit_user_toolkit_read**](ToolkitApi.md#toolkit_user_toolkit_read) | **GET** /toolkit/user_toolkit/{id}/ | 
[**toolkit_user_toolkit_update**](ToolkitApi.md#toolkit_user_toolkit_update) | **PUT** /toolkit/user_toolkit/{id}/ | 


# **toolkit_admin_toolkit_attribute_create**
> ToolkitAttribute toolkit_admin_toolkit_attribute_create(data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    data = autoppia_backend_client.ToolkitAttribute() # ToolkitAttribute | 

    try:
        api_response = api_instance.toolkit_admin_toolkit_attribute_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_attribute_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**ToolkitAttribute**](ToolkitAttribute.md)|  | 

### Return type

[**ToolkitAttribute**](ToolkitAttribute.md)

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

# **toolkit_admin_toolkit_attribute_delete**
> toolkit_admin_toolkit_attribute_delete(id)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit attribute.

    try:
        api_instance.toolkit_admin_toolkit_attribute_delete(id)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_attribute_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit attribute. | 

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

# **toolkit_admin_toolkit_attribute_list**
> list[ToolkitAttribute] toolkit_admin_toolkit_attribute_list()



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    
    try:
        api_response = api_instance.toolkit_admin_toolkit_attribute_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_attribute_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[ToolkitAttribute]**](ToolkitAttribute.md)

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

# **toolkit_admin_toolkit_attribute_partial_update**
> ToolkitAttribute toolkit_admin_toolkit_attribute_partial_update(id, data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit attribute.
data = autoppia_backend_client.ToolkitAttribute() # ToolkitAttribute | 

    try:
        api_response = api_instance.toolkit_admin_toolkit_attribute_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_attribute_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit attribute. | 
 **data** | [**ToolkitAttribute**](ToolkitAttribute.md)|  | 

### Return type

[**ToolkitAttribute**](ToolkitAttribute.md)

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

# **toolkit_admin_toolkit_attribute_read**
> ToolkitAttribute toolkit_admin_toolkit_attribute_read(id)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit attribute.

    try:
        api_response = api_instance.toolkit_admin_toolkit_attribute_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_attribute_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit attribute. | 

### Return type

[**ToolkitAttribute**](ToolkitAttribute.md)

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

# **toolkit_admin_toolkit_attribute_update**
> ToolkitAttribute toolkit_admin_toolkit_attribute_update(id, data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit attribute.
data = autoppia_backend_client.ToolkitAttribute() # ToolkitAttribute | 

    try:
        api_response = api_instance.toolkit_admin_toolkit_attribute_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_attribute_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit attribute. | 
 **data** | [**ToolkitAttribute**](ToolkitAttribute.md)|  | 

### Return type

[**ToolkitAttribute**](ToolkitAttribute.md)

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

# **toolkit_admin_toolkit_create**
> Toolkit toolkit_admin_toolkit_create(data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    data = autoppia_backend_client.Toolkit() # Toolkit | 

    try:
        api_response = api_instance.toolkit_admin_toolkit_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Toolkit**](Toolkit.md)|  | 

### Return type

[**Toolkit**](Toolkit.md)

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

# **toolkit_admin_toolkit_delete**
> toolkit_admin_toolkit_delete(id)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit.

    try:
        api_instance.toolkit_admin_toolkit_delete(id)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit. | 

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

# **toolkit_admin_toolkit_linked_integration_create**
> ToolkitLinkedIntegration toolkit_admin_toolkit_linked_integration_create(data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    data = autoppia_backend_client.ToolkitLinkedIntegration() # ToolkitLinkedIntegration | 

    try:
        api_response = api_instance.toolkit_admin_toolkit_linked_integration_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_linked_integration_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**ToolkitLinkedIntegration**](ToolkitLinkedIntegration.md)|  | 

### Return type

[**ToolkitLinkedIntegration**](ToolkitLinkedIntegration.md)

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

# **toolkit_admin_toolkit_linked_integration_delete**
> toolkit_admin_toolkit_linked_integration_delete(id)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit linked integration.

    try:
        api_instance.toolkit_admin_toolkit_linked_integration_delete(id)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_linked_integration_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit linked integration. | 

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

# **toolkit_admin_toolkit_linked_integration_list**
> list[ToolkitLinkedIntegration] toolkit_admin_toolkit_linked_integration_list()



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    
    try:
        api_response = api_instance.toolkit_admin_toolkit_linked_integration_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_linked_integration_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[ToolkitLinkedIntegration]**](ToolkitLinkedIntegration.md)

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

# **toolkit_admin_toolkit_linked_integration_partial_update**
> ToolkitLinkedIntegration toolkit_admin_toolkit_linked_integration_partial_update(id, data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit linked integration.
data = autoppia_backend_client.ToolkitLinkedIntegration() # ToolkitLinkedIntegration | 

    try:
        api_response = api_instance.toolkit_admin_toolkit_linked_integration_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_linked_integration_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit linked integration. | 
 **data** | [**ToolkitLinkedIntegration**](ToolkitLinkedIntegration.md)|  | 

### Return type

[**ToolkitLinkedIntegration**](ToolkitLinkedIntegration.md)

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

# **toolkit_admin_toolkit_linked_integration_read**
> ToolkitLinkedIntegration toolkit_admin_toolkit_linked_integration_read(id)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit linked integration.

    try:
        api_response = api_instance.toolkit_admin_toolkit_linked_integration_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_linked_integration_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit linked integration. | 

### Return type

[**ToolkitLinkedIntegration**](ToolkitLinkedIntegration.md)

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

# **toolkit_admin_toolkit_linked_integration_update**
> ToolkitLinkedIntegration toolkit_admin_toolkit_linked_integration_update(id, data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit linked integration.
data = autoppia_backend_client.ToolkitLinkedIntegration() # ToolkitLinkedIntegration | 

    try:
        api_response = api_instance.toolkit_admin_toolkit_linked_integration_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_linked_integration_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit linked integration. | 
 **data** | [**ToolkitLinkedIntegration**](ToolkitLinkedIntegration.md)|  | 

### Return type

[**ToolkitLinkedIntegration**](ToolkitLinkedIntegration.md)

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

# **toolkit_admin_toolkit_list**
> list[Toolkit] toolkit_admin_toolkit_list()



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    
    try:
        api_response = api_instance.toolkit_admin_toolkit_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[Toolkit]**](Toolkit.md)

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

# **toolkit_admin_toolkit_partial_update**
> Toolkit toolkit_admin_toolkit_partial_update(id, data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit.
data = autoppia_backend_client.Toolkit() # Toolkit | 

    try:
        api_response = api_instance.toolkit_admin_toolkit_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit. | 
 **data** | [**Toolkit**](Toolkit.md)|  | 

### Return type

[**Toolkit**](Toolkit.md)

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

# **toolkit_admin_toolkit_read**
> Toolkit toolkit_admin_toolkit_read(id)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit.

    try:
        api_response = api_instance.toolkit_admin_toolkit_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit. | 

### Return type

[**Toolkit**](Toolkit.md)

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

# **toolkit_admin_toolkit_update**
> Toolkit toolkit_admin_toolkit_update(id, data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit.
data = autoppia_backend_client.Toolkit() # Toolkit | 

    try:
        api_response = api_instance.toolkit_admin_toolkit_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_admin_toolkit_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit. | 
 **data** | [**Toolkit**](Toolkit.md)|  | 

### Return type

[**Toolkit**](Toolkit.md)

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

# **toolkit_tool_create**
> Tool toolkit_tool_create(data)



Create a new tool

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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    data = autoppia_backend_client.Tool() # Tool | 

    try:
        api_response = api_instance.toolkit_tool_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_tool_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**Tool**](Tool.md)|  | 

### Return type

[**Tool**](Tool.md)

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

# **toolkit_tool_delete**
> toolkit_tool_delete(id)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this tool.

    try:
        api_instance.toolkit_tool_delete(id)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_tool_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this tool. | 

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

# **toolkit_tool_list**
> list[Tool] toolkit_tool_list()



Get a list of tools

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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    
    try:
        api_response = api_instance.toolkit_tool_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_tool_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[Tool]**](Tool.md)

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

# **toolkit_tool_partial_update**
> Tool toolkit_tool_partial_update(id, data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this tool.
data = autoppia_backend_client.Tool() # Tool | 

    try:
        api_response = api_instance.toolkit_tool_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_tool_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this tool. | 
 **data** | [**Tool**](Tool.md)|  | 

### Return type

[**Tool**](Tool.md)

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

# **toolkit_tool_read**
> Tool toolkit_tool_read(id)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this tool.

    try:
        api_response = api_instance.toolkit_tool_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_tool_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this tool. | 

### Return type

[**Tool**](Tool.md)

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

# **toolkit_tool_update**
> Tool toolkit_tool_update(id, data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this tool.
data = autoppia_backend_client.Tool() # Tool | 

    try:
        api_response = api_instance.toolkit_tool_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_tool_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this tool. | 
 **data** | [**Tool**](Tool.md)|  | 

### Return type

[**Tool**](Tool.md)

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

# **toolkit_toolkit_list**
> list[ListToolkit] toolkit_toolkit_list()



Get a list of toolkits

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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    
    try:
        api_response = api_instance.toolkit_toolkit_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_toolkit_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[ListToolkit]**](ListToolkit.md)

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

# **toolkit_toolkit_read**
> ListToolkit toolkit_toolkit_read(id)



Retrieve a toolkit by ID

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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this toolkit.

    try:
        api_response = api_instance.toolkit_toolkit_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_toolkit_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this toolkit. | 

### Return type

[**ListToolkit**](ListToolkit.md)

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

# **toolkit_user_configuration_create**
> UserConfiguration toolkit_user_configuration_create(data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    data = autoppia_backend_client.UserConfiguration() # UserConfiguration | 

    try:
        api_response = api_instance.toolkit_user_configuration_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_configuration_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**UserConfiguration**](UserConfiguration.md)|  | 

### Return type

[**UserConfiguration**](UserConfiguration.md)

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

# **toolkit_user_configuration_delete**
> toolkit_user_configuration_delete(id)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this user configuration.

    try:
        api_instance.toolkit_user_configuration_delete(id)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_configuration_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user configuration. | 

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

# **toolkit_user_configuration_list**
> list[ListUserConfiguration] toolkit_user_configuration_list()



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    
    try:
        api_response = api_instance.toolkit_user_configuration_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_configuration_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[ListUserConfiguration]**](ListUserConfiguration.md)

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

# **toolkit_user_configuration_partial_update**
> UserConfiguration toolkit_user_configuration_partial_update(id, data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this user configuration.
data = autoppia_backend_client.UserConfiguration() # UserConfiguration | 

    try:
        api_response = api_instance.toolkit_user_configuration_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_configuration_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user configuration. | 
 **data** | [**UserConfiguration**](UserConfiguration.md)|  | 

### Return type

[**UserConfiguration**](UserConfiguration.md)

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

# **toolkit_user_configuration_read**
> ListUserConfiguration toolkit_user_configuration_read(id)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this user configuration.

    try:
        api_response = api_instance.toolkit_user_configuration_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_configuration_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user configuration. | 

### Return type

[**ListUserConfiguration**](ListUserConfiguration.md)

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

# **toolkit_user_configuration_update**
> UserConfiguration toolkit_user_configuration_update(id, data)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this user configuration.
data = autoppia_backend_client.UserConfiguration() # UserConfiguration | 

    try:
        api_response = api_instance.toolkit_user_configuration_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_configuration_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user configuration. | 
 **data** | [**UserConfiguration**](UserConfiguration.md)|  | 

### Return type

[**UserConfiguration**](UserConfiguration.md)

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

# **toolkit_user_toolkit_create**
> UserToolkit toolkit_user_toolkit_create(data)



Create a new user toolkit

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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    data = autoppia_backend_client.UserToolkit() # UserToolkit | 

    try:
        api_response = api_instance.toolkit_user_toolkit_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_toolkit_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**UserToolkit**](UserToolkit.md)|  | 

### Return type

[**UserToolkit**](UserToolkit.md)

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

# **toolkit_user_toolkit_delete**
> toolkit_user_toolkit_delete(id)



Delete a user toolkit by its ID

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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this user toolkit.

    try:
        api_instance.toolkit_user_toolkit_delete(id)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_toolkit_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user toolkit. | 

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

# **toolkit_user_toolkit_list**
> list[ListUserToolkit] toolkit_user_toolkit_list()



Get list of user toolkits.

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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    
    try:
        api_response = api_instance.toolkit_user_toolkit_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_toolkit_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[ListUserToolkit]**](ListUserToolkit.md)

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

# **toolkit_user_toolkit_partial_update**
> UserToolkit toolkit_user_toolkit_partial_update(id, data)



Partially update an existing user toolkit

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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this user toolkit.
data = autoppia_backend_client.UserToolkit() # UserToolkit | 

    try:
        api_response = api_instance.toolkit_user_toolkit_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_toolkit_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user toolkit. | 
 **data** | [**UserToolkit**](UserToolkit.md)|  | 

### Return type

[**UserToolkit**](UserToolkit.md)

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

# **toolkit_user_toolkit_read**
> ListUserToolkit toolkit_user_toolkit_read(id)



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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this user toolkit.

    try:
        api_response = api_instance.toolkit_user_toolkit_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_toolkit_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user toolkit. | 

### Return type

[**ListUserToolkit**](ListUserToolkit.md)

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

# **toolkit_user_toolkit_update**
> UserToolkit toolkit_user_toolkit_update(id, data)



Update an existing user toolkit

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
    api_instance = autoppia_backend_client.ToolkitApi(api_client)
    id = 56 # int | A unique integer value identifying this user toolkit.
data = autoppia_backend_client.UserToolkit() # UserToolkit | 

    try:
        api_response = api_instance.toolkit_user_toolkit_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling ToolkitApi->toolkit_user_toolkit_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this user toolkit. | 
 **data** | [**UserToolkit**](UserToolkit.md)|  | 

### Return type

[**UserToolkit**](UserToolkit.md)

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

