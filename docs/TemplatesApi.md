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
[**templates_worker_templates_get_deployed_count**](TemplatesApi.md#templates_worker_templates_get_deployed_count) | **GET** /templates/worker-templates/getDeployedCount/ | 
[**templates_worker_templates_list**](TemplatesApi.md#templates_worker_templates_list) | **GET** /templates/worker-templates/ | 
[**templates_worker_templates_my_favorits_count**](TemplatesApi.md#templates_worker_templates_my_favorits_count) | **GET** /templates/worker-templates/myFavoritsCount/ | 
[**templates_worker_templates_partial_update**](TemplatesApi.md#templates_worker_templates_partial_update) | **PATCH** /templates/worker-templates/{id}/ | 
[**templates_worker_templates_read**](TemplatesApi.md#templates_worker_templates_read) | **GET** /templates/worker-templates/{id}/ | 
[**templates_worker_templates_unfavorite**](TemplatesApi.md#templates_worker_templates_unfavorite) | **DELETE** /templates/worker-templates/{id}/unfavorite/ | 
[**templates_worker_templates_update**](TemplatesApi.md#templates_worker_templates_update) | **PUT** /templates/worker-templates/{id}/ | 


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
> WorkerTemplate templates_worker_templates_create(title, description, repo, favorited_by=favorited_by, categories=categories, image=image, docker_image=docker_image, hourly_rate=hourly_rate, llm_provider=llm_provider, llm=llm, integrations_categories=integrations_categories, vectorstore_provider=vectorstore_provider, agentic_framework=agentic_framework, firewall=firewall, gpu=gpu, gpu_type=gpu_type, demo_video=demo_video)



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
    title = 'title_example' # str | 
description = 'description_example' # str | 
repo = 'repo_example' # str | 
favorited_by = 56 # list[int] |  (optional)
categories = 56 # list[int] |  (optional)
image = '/path/to/file' # file |  (optional)
docker_image = 'docker_image_example' # str |  (optional)
hourly_rate = 'hourly_rate_example' # str |  (optional)
llm_provider = 'llm_provider_example' # str |  (optional)
llm = 'llm_example' # str |  (optional)
integrations_categories = 'integrations_categories_example' # str |  (optional)
vectorstore_provider = 'vectorstore_provider_example' # str |  (optional)
agentic_framework = 'agentic_framework_example' # str |  (optional)
firewall = 'firewall_example' # str |  (optional)
gpu = True # bool |  (optional)
gpu_type = 'gpu_type_example' # str |  (optional)
demo_video = '/path/to/file' # file |  (optional)

    try:
        api_response = api_instance.templates_worker_templates_create(title, description, repo, favorited_by=favorited_by, categories=categories, image=image, docker_image=docker_image, hourly_rate=hourly_rate, llm_provider=llm_provider, llm=llm, integrations_categories=integrations_categories, vectorstore_provider=vectorstore_provider, agentic_framework=agentic_framework, firewall=firewall, gpu=gpu, gpu_type=gpu_type, demo_video=demo_video)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_create: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **title** | **str**|  | 
 **description** | **str**|  | 
 **repo** | **str**|  | 
 **favorited_by** | [**list[int]**](int.md)|  | [optional] 
 **categories** | [**list[int]**](int.md)|  | [optional] 
 **image** | **file**|  | [optional] 
 **docker_image** | **str**|  | [optional] 
 **hourly_rate** | **str**|  | [optional] 
 **llm_provider** | **str**|  | [optional] 
 **llm** | **str**|  | [optional] 
 **integrations_categories** | **str**|  | [optional] 
 **vectorstore_provider** | **str**|  | [optional] 
 **agentic_framework** | **str**|  | [optional] 
 **firewall** | **str**|  | [optional] 
 **gpu** | **bool**|  | [optional] 
 **gpu_type** | **str**|  | [optional] 
 **demo_video** | **file**|  | [optional] 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: multipart/form-data, application/x-www-form-urlencoded
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
> WorkerTemplate templates_worker_templates_deploy(id, title, description, repo, favorited_by=favorited_by, categories=categories, image=image, docker_image=docker_image, hourly_rate=hourly_rate, llm_provider=llm_provider, llm=llm, integrations_categories=integrations_categories, vectorstore_provider=vectorstore_provider, agentic_framework=agentic_framework, firewall=firewall, gpu=gpu, gpu_type=gpu_type, demo_video=demo_video)



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
title = 'title_example' # str | 
description = 'description_example' # str | 
repo = 'repo_example' # str | 
favorited_by = 56 # list[int] |  (optional)
categories = 56 # list[int] |  (optional)
image = '/path/to/file' # file |  (optional)
docker_image = 'docker_image_example' # str |  (optional)
hourly_rate = 'hourly_rate_example' # str |  (optional)
llm_provider = 'llm_provider_example' # str |  (optional)
llm = 'llm_example' # str |  (optional)
integrations_categories = 'integrations_categories_example' # str |  (optional)
vectorstore_provider = 'vectorstore_provider_example' # str |  (optional)
agentic_framework = 'agentic_framework_example' # str |  (optional)
firewall = 'firewall_example' # str |  (optional)
gpu = True # bool |  (optional)
gpu_type = 'gpu_type_example' # str |  (optional)
demo_video = '/path/to/file' # file |  (optional)

    try:
        api_response = api_instance.templates_worker_templates_deploy(id, title, description, repo, favorited_by=favorited_by, categories=categories, image=image, docker_image=docker_image, hourly_rate=hourly_rate, llm_provider=llm_provider, llm=llm, integrations_categories=integrations_categories, vectorstore_provider=vectorstore_provider, agentic_framework=agentic_framework, firewall=firewall, gpu=gpu, gpu_type=gpu_type, demo_video=demo_video)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_deploy: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker template. | 
 **title** | **str**|  | 
 **description** | **str**|  | 
 **repo** | **str**|  | 
 **favorited_by** | [**list[int]**](int.md)|  | [optional] 
 **categories** | [**list[int]**](int.md)|  | [optional] 
 **image** | **file**|  | [optional] 
 **docker_image** | **str**|  | [optional] 
 **hourly_rate** | **str**|  | [optional] 
 **llm_provider** | **str**|  | [optional] 
 **llm** | **str**|  | [optional] 
 **integrations_categories** | **str**|  | [optional] 
 **vectorstore_provider** | **str**|  | [optional] 
 **agentic_framework** | **str**|  | [optional] 
 **firewall** | **str**|  | [optional] 
 **gpu** | **bool**|  | [optional] 
 **gpu_type** | **str**|  | [optional] 
 **demo_video** | **file**|  | [optional] 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: multipart/form-data, application/x-www-form-urlencoded
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **templates_worker_templates_favorite**
> WorkerTemplate templates_worker_templates_favorite(id, title, description, repo, favorited_by=favorited_by, categories=categories, image=image, docker_image=docker_image, hourly_rate=hourly_rate, llm_provider=llm_provider, llm=llm, integrations_categories=integrations_categories, vectorstore_provider=vectorstore_provider, agentic_framework=agentic_framework, firewall=firewall, gpu=gpu, gpu_type=gpu_type, demo_video=demo_video)



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
title = 'title_example' # str | 
description = 'description_example' # str | 
repo = 'repo_example' # str | 
favorited_by = 56 # list[int] |  (optional)
categories = 56 # list[int] |  (optional)
image = '/path/to/file' # file |  (optional)
docker_image = 'docker_image_example' # str |  (optional)
hourly_rate = 'hourly_rate_example' # str |  (optional)
llm_provider = 'llm_provider_example' # str |  (optional)
llm = 'llm_example' # str |  (optional)
integrations_categories = 'integrations_categories_example' # str |  (optional)
vectorstore_provider = 'vectorstore_provider_example' # str |  (optional)
agentic_framework = 'agentic_framework_example' # str |  (optional)
firewall = 'firewall_example' # str |  (optional)
gpu = True # bool |  (optional)
gpu_type = 'gpu_type_example' # str |  (optional)
demo_video = '/path/to/file' # file |  (optional)

    try:
        api_response = api_instance.templates_worker_templates_favorite(id, title, description, repo, favorited_by=favorited_by, categories=categories, image=image, docker_image=docker_image, hourly_rate=hourly_rate, llm_provider=llm_provider, llm=llm, integrations_categories=integrations_categories, vectorstore_provider=vectorstore_provider, agentic_framework=agentic_framework, firewall=firewall, gpu=gpu, gpu_type=gpu_type, demo_video=demo_video)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_favorite: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker template. | 
 **title** | **str**|  | 
 **description** | **str**|  | 
 **repo** | **str**|  | 
 **favorited_by** | [**list[int]**](int.md)|  | [optional] 
 **categories** | [**list[int]**](int.md)|  | [optional] 
 **image** | **file**|  | [optional] 
 **docker_image** | **str**|  | [optional] 
 **hourly_rate** | **str**|  | [optional] 
 **llm_provider** | **str**|  | [optional] 
 **llm** | **str**|  | [optional] 
 **integrations_categories** | **str**|  | [optional] 
 **vectorstore_provider** | **str**|  | [optional] 
 **agentic_framework** | **str**|  | [optional] 
 **firewall** | **str**|  | [optional] 
 **gpu** | **bool**|  | [optional] 
 **gpu_type** | **str**|  | [optional] 
 **demo_video** | **file**|  | [optional] 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: multipart/form-data, application/x-www-form-urlencoded
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
> WorkerTemplate templates_worker_templates_partial_update(id, title, description, repo, favorited_by=favorited_by, categories=categories, image=image, docker_image=docker_image, hourly_rate=hourly_rate, llm_provider=llm_provider, llm=llm, integrations_categories=integrations_categories, vectorstore_provider=vectorstore_provider, agentic_framework=agentic_framework, firewall=firewall, gpu=gpu, gpu_type=gpu_type, demo_video=demo_video)



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
title = 'title_example' # str | 
description = 'description_example' # str | 
repo = 'repo_example' # str | 
favorited_by = 56 # list[int] |  (optional)
categories = 56 # list[int] |  (optional)
image = '/path/to/file' # file |  (optional)
docker_image = 'docker_image_example' # str |  (optional)
hourly_rate = 'hourly_rate_example' # str |  (optional)
llm_provider = 'llm_provider_example' # str |  (optional)
llm = 'llm_example' # str |  (optional)
integrations_categories = 'integrations_categories_example' # str |  (optional)
vectorstore_provider = 'vectorstore_provider_example' # str |  (optional)
agentic_framework = 'agentic_framework_example' # str |  (optional)
firewall = 'firewall_example' # str |  (optional)
gpu = True # bool |  (optional)
gpu_type = 'gpu_type_example' # str |  (optional)
demo_video = '/path/to/file' # file |  (optional)

    try:
        api_response = api_instance.templates_worker_templates_partial_update(id, title, description, repo, favorited_by=favorited_by, categories=categories, image=image, docker_image=docker_image, hourly_rate=hourly_rate, llm_provider=llm_provider, llm=llm, integrations_categories=integrations_categories, vectorstore_provider=vectorstore_provider, agentic_framework=agentic_framework, firewall=firewall, gpu=gpu, gpu_type=gpu_type, demo_video=demo_video)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_partial_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker template. | 
 **title** | **str**|  | 
 **description** | **str**|  | 
 **repo** | **str**|  | 
 **favorited_by** | [**list[int]**](int.md)|  | [optional] 
 **categories** | [**list[int]**](int.md)|  | [optional] 
 **image** | **file**|  | [optional] 
 **docker_image** | **str**|  | [optional] 
 **hourly_rate** | **str**|  | [optional] 
 **llm_provider** | **str**|  | [optional] 
 **llm** | **str**|  | [optional] 
 **integrations_categories** | **str**|  | [optional] 
 **vectorstore_provider** | **str**|  | [optional] 
 **agentic_framework** | **str**|  | [optional] 
 **firewall** | **str**|  | [optional] 
 **gpu** | **bool**|  | [optional] 
 **gpu_type** | **str**|  | [optional] 
 **demo_video** | **file**|  | [optional] 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: multipart/form-data, application/x-www-form-urlencoded
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
> WorkerTemplate templates_worker_templates_update(id, title, description, repo, favorited_by=favorited_by, categories=categories, image=image, docker_image=docker_image, hourly_rate=hourly_rate, llm_provider=llm_provider, llm=llm, integrations_categories=integrations_categories, vectorstore_provider=vectorstore_provider, agentic_framework=agentic_framework, firewall=firewall, gpu=gpu, gpu_type=gpu_type, demo_video=demo_video)



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
title = 'title_example' # str | 
description = 'description_example' # str | 
repo = 'repo_example' # str | 
favorited_by = 56 # list[int] |  (optional)
categories = 56 # list[int] |  (optional)
image = '/path/to/file' # file |  (optional)
docker_image = 'docker_image_example' # str |  (optional)
hourly_rate = 'hourly_rate_example' # str |  (optional)
llm_provider = 'llm_provider_example' # str |  (optional)
llm = 'llm_example' # str |  (optional)
integrations_categories = 'integrations_categories_example' # str |  (optional)
vectorstore_provider = 'vectorstore_provider_example' # str |  (optional)
agentic_framework = 'agentic_framework_example' # str |  (optional)
firewall = 'firewall_example' # str |  (optional)
gpu = True # bool |  (optional)
gpu_type = 'gpu_type_example' # str |  (optional)
demo_video = '/path/to/file' # file |  (optional)

    try:
        api_response = api_instance.templates_worker_templates_update(id, title, description, repo, favorited_by=favorited_by, categories=categories, image=image, docker_image=docker_image, hourly_rate=hourly_rate, llm_provider=llm_provider, llm=llm, integrations_categories=integrations_categories, vectorstore_provider=vectorstore_provider, agentic_framework=agentic_framework, firewall=firewall, gpu=gpu, gpu_type=gpu_type, demo_video=demo_video)
        pprint(api_response)
    except ApiException as e:
        print("Exception when calling TemplatesApi->templates_worker_templates_update: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| A unique integer value identifying this worker template. | 
 **title** | **str**|  | 
 **description** | **str**|  | 
 **repo** | **str**|  | 
 **favorited_by** | [**list[int]**](int.md)|  | [optional] 
 **categories** | [**list[int]**](int.md)|  | [optional] 
 **image** | **file**|  | [optional] 
 **docker_image** | **str**|  | [optional] 
 **hourly_rate** | **str**|  | [optional] 
 **llm_provider** | **str**|  | [optional] 
 **llm** | **str**|  | [optional] 
 **integrations_categories** | **str**|  | [optional] 
 **vectorstore_provider** | **str**|  | [optional] 
 **agentic_framework** | **str**|  | [optional] 
 **firewall** | **str**|  | [optional] 
 **gpu** | **bool**|  | [optional] 
 **gpu_type** | **str**|  | [optional] 
 **demo_video** | **file**|  | [optional] 

### Return type

[**WorkerTemplate**](WorkerTemplate.md)

### Authorization

[Basic](../README.md#Basic)

### HTTP request headers

 - **Content-Type**: multipart/form-data, application/x-www-form-urlencoded
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

