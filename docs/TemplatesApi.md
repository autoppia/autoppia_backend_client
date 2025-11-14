# autoppia_backend_client.TemplatesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**templates_categories_list**](TemplatesApi.md#templates_categories_list) | **GET** /templates/categories/ | 
[**templates_categories_read**](TemplatesApi.md#templates_categories_read) | **GET** /templates/categories/{id}/ | 
[**templates_worker_templates_count**](TemplatesApi.md#templates_worker_templates_count) | **GET** /templates/worker-templates/count/ | 
[**templates_worker_templates_create**](TemplatesApi.md#templates_worker_templates_create) | **POST** /templates/worker-templates/ | 
[**templates_worker_templates_delete**](TemplatesApi.md#templates_worker_templates_delete) | **DELETE** /templates/worker-templates/{id}/ | 
[**templates_worker_templates_deploy**](TemplatesApi.md#templates_worker_templates_deploy) | **POST** /templates/worker-templates/{id}/deploy/ | 
[**templates_worker_templates_favorite**](TemplatesApi.md#templates_worker_templates_favorite) | **POST** /templates/worker-templates/{id}/favorite/ | 
[**templates_worker_templates_favorites**](TemplatesApi.md#templates_worker_templates_favorites) | **GET** /templates/worker-templates/favorites/ | 
[**templates_worker_templates_filtered_templates**](TemplatesApi.md#templates_worker_templates_filtered_templates) | **GET** /templates/worker-templates/filteredTemplates/ | 
[**templates_worker_templates_generate_ecr_credentials**](TemplatesApi.md#templates_worker_templates_generate_ecr_credentials) | **POST** /templates/worker-templates/generate_ecr_credentials/ | 
[**templates_worker_templates_generate_upload_urls**](TemplatesApi.md#templates_worker_templates_generate_upload_urls) | **POST** /templates/worker-templates/generate_upload_urls/ | 
[**templates_worker_templates_get_deployed_count**](TemplatesApi.md#templates_worker_templates_get_deployed_count) | **GET** /templates/worker-templates/getDeployedCount/ | 
[**templates_worker_templates_list**](TemplatesApi.md#templates_worker_templates_list) | **GET** /templates/worker-templates/ | 
[**templates_worker_templates_my_favorits_count**](TemplatesApi.md#templates_worker_templates_my_favorits_count) | **GET** /templates/worker-templates/myFavoritsCount/ | 
[**templates_worker_templates_partial_update**](TemplatesApi.md#templates_worker_templates_partial_update) | **PATCH** /templates/worker-templates/{id}/ | 
[**templates_worker_templates_read**](TemplatesApi.md#templates_worker_templates_read) | **GET** /templates/worker-templates/{id}/ | 
[**templates_worker_templates_test_s3_connection**](TemplatesApi.md#templates_worker_templates_test_s3_connection) | **GET** /templates/worker-templates/test_s3_connection/ | 
[**templates_worker_templates_unfavorite**](TemplatesApi.md#templates_worker_templates_unfavorite) | **DELETE** /templates/worker-templates/{id}/unfavorite/ | 
[**templates_worker_templates_update**](TemplatesApi.md#templates_worker_templates_update) | **PUT** /templates/worker-templates/{id}/ | 
[**templates_worker_templates_upload_file**](TemplatesApi.md#templates_worker_templates_upload_file) | **POST** /templates/worker-templates/upload_file/ | 


# **templates_categories_list**
> list[Categories] templates_categories_list()



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    
    try:
        api_response = api_instance.templates_categories_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_categories_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[Categories]**](Categories.md)

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

# **templates_categories_read**
> Categories templates_categories_read(id)



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    id = 56 # int | A unique integer value identifying this categories.

    try:
        api_response = api_instance.templates_categories_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_categories_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this categories. | 

### Return type

[**Categories**](Categories.md)

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

# **templates_worker_templates_count**
> list[WorkerTemplate] templates_worker_templates_count()



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    
    try:
        api_response = api_instance.templates_worker_templates_count()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_count: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[WorkerTemplate]**](WorkerTemplate.md)

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

# **templates_worker_templates_create**
> WorkerTemplate templates_worker_templates_create(data)



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    data = autoppia_backend_client.WorkerTemplate() # WorkerTemplate | 

    try:
        api_response = api_instance.templates_worker_templates_create(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**WorkerTemplate**](WorkerTemplate.md)|  | 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

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

# **templates_worker_templates_delete**
> templates_worker_templates_delete(id)



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    id = 56 # int | A unique integer value identifying this worker template.

    try:
        api_instance.templates_worker_templates_delete(id)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_delete: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker template. | 

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

# **templates_worker_templates_deploy**
> WorkerTemplate templates_worker_templates_deploy(id, data)



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    id = 56 # int | A unique integer value identifying this worker template.
data = autoppia_backend_client.WorkerTemplate() # WorkerTemplate | 

    try:
        api_response = api_instance.templates_worker_templates_deploy(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_deploy: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker template. | 
 **data** | [**WorkerTemplate**](WorkerTemplate.md)|  | 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

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

# **templates_worker_templates_favorite**
> WorkerTemplate templates_worker_templates_favorite(id, data)



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    id = 56 # int | A unique integer value identifying this worker template.
data = autoppia_backend_client.WorkerTemplate() # WorkerTemplate | 

    try:
        api_response = api_instance.templates_worker_templates_favorite(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_favorite: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker template. | 
 **data** | [**WorkerTemplate**](WorkerTemplate.md)|  | 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

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

# **templates_worker_templates_favorites**
> list[WorkerTemplate] templates_worker_templates_favorites()



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    
    try:
        api_response = api_instance.templates_worker_templates_favorites()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_favorites: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[WorkerTemplate]**](WorkerTemplate.md)

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

# **templates_worker_templates_filtered_templates**
> list[WorkerTemplate] templates_worker_templates_filtered_templates()



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    
    try:
        api_response = api_instance.templates_worker_templates_filtered_templates()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_filtered_templates: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[WorkerTemplate]**](WorkerTemplate.md)

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

# **templates_worker_templates_generate_ecr_credentials**
> WorkerTemplate templates_worker_templates_generate_ecr_credentials(data)



Generate temporary AWS credentials for ECR push access ONLY Fixed 1-hour duration for maximum security

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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    data = autoppia_backend_client.WorkerTemplate() # WorkerTemplate | 

    try:
        api_response = api_instance.templates_worker_templates_generate_ecr_credentials(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_generate_ecr_credentials: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**WorkerTemplate**](WorkerTemplate.md)|  | 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

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

# **templates_worker_templates_generate_upload_urls**
> WorkerTemplate templates_worker_templates_generate_upload_urls(data)



Generate presigned S3 URLs for direct client upload

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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    data = autoppia_backend_client.WorkerTemplate() # WorkerTemplate | 

    try:
        api_response = api_instance.templates_worker_templates_generate_upload_urls(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_generate_upload_urls: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**WorkerTemplate**](WorkerTemplate.md)|  | 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

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

# **templates_worker_templates_get_deployed_count**
> list[WorkerTemplate] templates_worker_templates_get_deployed_count()



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    
    try:
        api_response = api_instance.templates_worker_templates_get_deployed_count()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_get_deployed_count: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[WorkerTemplate]**](WorkerTemplate.md)

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

# **templates_worker_templates_list**
> list[WorkerTemplate] templates_worker_templates_list()



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    
    try:
        api_response = api_instance.templates_worker_templates_list()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_list: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[WorkerTemplate]**](WorkerTemplate.md)

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

# **templates_worker_templates_my_favorits_count**
> list[WorkerTemplate] templates_worker_templates_my_favorits_count()



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    
    try:
        api_response = api_instance.templates_worker_templates_my_favorits_count()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_my_favorits_count: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[WorkerTemplate]**](WorkerTemplate.md)

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

# **templates_worker_templates_partial_update**
> WorkerTemplate templates_worker_templates_partial_update(id, data)



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    id = 56 # int | A unique integer value identifying this worker template.
data = autoppia_backend_client.WorkerTemplate() # WorkerTemplate | 

    try:
        api_response = api_instance.templates_worker_templates_partial_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker template. | 
 **data** | [**WorkerTemplate**](WorkerTemplate.md)|  | 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

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

# **templates_worker_templates_read**
> WorkerTemplate templates_worker_templates_read(id)



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    id = 56 # int | A unique integer value identifying this worker template.

    try:
        api_response = api_instance.templates_worker_templates_read(id)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_read: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker template. | 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

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

# **templates_worker_templates_test_s3_connection**
> list[WorkerTemplate] templates_worker_templates_test_s3_connection()



Test S3 connection and configuration

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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    
    try:
        api_response = api_instance.templates_worker_templates_test_s3_connection()
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_test_s3_connection: %s\n" % e)
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**list[WorkerTemplate]**](WorkerTemplate.md)

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

# **templates_worker_templates_unfavorite**
> templates_worker_templates_unfavorite(id)



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    id = 56 # int | A unique integer value identifying this worker template.

    try:
        api_instance.templates_worker_templates_unfavorite(id)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_unfavorite: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker template. | 

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

# **templates_worker_templates_update**
> WorkerTemplate templates_worker_templates_update(id, data)



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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    id = 56 # int | A unique integer value identifying this worker template.
data = autoppia_backend_client.WorkerTemplate() # WorkerTemplate | 

    try:
        api_response = api_instance.templates_worker_templates_update(id, data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker template. | 
 **data** | [**WorkerTemplate**](WorkerTemplate.md)|  | 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

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

# **templates_worker_templates_upload_file**
> WorkerTemplate templates_worker_templates_upload_file(data)



Upload a single file to S3 and return the URL

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
    api_instance = autoppia_backend_client.TemplatesApi(api_client)
    data = autoppia_backend_client.WorkerTemplate() # WorkerTemplate | 

    try:
        api_response = api_instance.templates_worker_templates_upload_file(data)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_upload_file: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **data** | [**WorkerTemplate**](WorkerTemplate.md)|  | 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

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

