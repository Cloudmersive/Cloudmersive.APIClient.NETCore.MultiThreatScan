# Cloudmersive.APIClient.NETCore.MultiThreatScan.Api.MultiThreatApi

All URIs are relative to *http://localhost*

| Method | HTTP request | Description |
|--------|--------------|-------------|
| [**MultiThreatScanFilePost**](MultiThreatApi.md#multithreatscanfilepost) | **POST** /multi-threat-scan/file | Scan a file for multiple threat types including viruses, NSFW, AI-generated content, fraud, phishing, spam, DLP, and policy violations in a single API call. |
| [**MultiThreatScanTextPost**](MultiThreatApi.md#multithreatscantextpost) | **POST** /multi-threat-scan/text | Scan text for multiple threat types including viruses, phishing, spam, DLP, and policy violations in a single API call. |
| [**MultiThreatScanUrlPost**](MultiThreatApi.md#multithreatscanurlpost) | **POST** /multi-threat-scan/url | Scan a URL for multiple threat types including viruses, phishing, and policy violations in a single API call. Optionally download and scan the file at the URL. |

<a id="multithreatscanfilepost"></a>
# **MultiThreatScanFilePost**
> MultiThreatFileResponse MultiThreatScanFilePost (System.IO.Stream inputFile, string config = null)

Scan a file for multiple threat types including viruses, NSFW, AI-generated content, fraud, phishing, spam, DLP, and policy violations in a single API call.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Cloudmersive.APIClient.NETCore.MultiThreatScan.Api;
using Cloudmersive.APIClient.NETCore.MultiThreatScan.Client;
using Cloudmersive.APIClient.NETCore.MultiThreatScan.Model;

namespace Example
{
    public class MultiThreatScanFilePostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "http://localhost";
            // Configure API key authorization: Apikey
            config.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new MultiThreatApi(config);
            var inputFile = new System.IO.MemoryStream(System.IO.File.ReadAllBytes("/path/to/file.txt"));  // System.IO.Stream | The file to scan
            var config = "config_example";  // string | Optional JSON scan configuration (optional) 

            try
            {
                // Scan a file for multiple threat types including viruses, NSFW, AI-generated content, fraud, phishing, spam, DLP, and policy violations in a single API call.
                MultiThreatFileResponse result = apiInstance.MultiThreatScanFilePost(inputFile, config);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MultiThreatApi.MultiThreatScanFilePost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MultiThreatScanFilePostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Scan a file for multiple threat types including viruses, NSFW, AI-generated content, fraud, phishing, spam, DLP, and policy violations in a single API call.
    ApiResponse<MultiThreatFileResponse> response = apiInstance.MultiThreatScanFilePostWithHttpInfo(inputFile, config);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MultiThreatApi.MultiThreatScanFilePostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **inputFile** | **System.IO.Stream****System.IO.Stream** | The file to scan |  |
| **config** | **string** | Optional JSON scan configuration | [optional]  |

### Return type

[**MultiThreatFileResponse**](MultiThreatFileResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="multithreatscantextpost"></a>
# **MultiThreatScanTextPost**
> MultiThreatTextResponse MultiThreatScanTextPost (MultiThreatTextRequest body = null)

Scan text for multiple threat types including viruses, phishing, spam, DLP, and policy violations in a single API call.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Cloudmersive.APIClient.NETCore.MultiThreatScan.Api;
using Cloudmersive.APIClient.NETCore.MultiThreatScan.Client;
using Cloudmersive.APIClient.NETCore.MultiThreatScan.Model;

namespace Example
{
    public class MultiThreatScanTextPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "http://localhost";
            // Configure API key authorization: Apikey
            config.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new MultiThreatApi(config);
            var body = new MultiThreatTextRequest(); // MultiThreatTextRequest | Text scan request with content and scan configuration (optional) 

            try
            {
                // Scan text for multiple threat types including viruses, phishing, spam, DLP, and policy violations in a single API call.
                MultiThreatTextResponse result = apiInstance.MultiThreatScanTextPost(body);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MultiThreatApi.MultiThreatScanTextPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MultiThreatScanTextPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Scan text for multiple threat types including viruses, phishing, spam, DLP, and policy violations in a single API call.
    ApiResponse<MultiThreatTextResponse> response = apiInstance.MultiThreatScanTextPostWithHttpInfo(body);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MultiThreatApi.MultiThreatScanTextPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **body** | [**MultiThreatTextRequest**](MultiThreatTextRequest.md) | Text scan request with content and scan configuration | [optional]  |

### Return type

[**MultiThreatTextResponse**](MultiThreatTextResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

<a id="multithreatscanurlpost"></a>
# **MultiThreatScanUrlPost**
> MultiThreatUrlResponse MultiThreatScanUrlPost (MultiThreatUrlRequest body = null)

Scan a URL for multiple threat types including viruses, phishing, and policy violations in a single API call. Optionally download and scan the file at the URL.

### Example
```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Cloudmersive.APIClient.NETCore.MultiThreatScan.Api;
using Cloudmersive.APIClient.NETCore.MultiThreatScan.Client;
using Cloudmersive.APIClient.NETCore.MultiThreatScan.Model;

namespace Example
{
    public class MultiThreatScanUrlPostExample
    {
        public static void Main()
        {
            Configuration config = new Configuration();
            config.BasePath = "http://localhost";
            // Configure API key authorization: Apikey
            config.AddApiKey("Apikey", "YOUR_API_KEY");
            // Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
            // config.AddApiKeyPrefix("Apikey", "Bearer");

            var apiInstance = new MultiThreatApi(config);
            var body = new MultiThreatUrlRequest(); // MultiThreatUrlRequest | URL scan request with URL and scan configuration (optional) 

            try
            {
                // Scan a URL for multiple threat types including viruses, phishing, and policy violations in a single API call. Optionally download and scan the file at the URL.
                MultiThreatUrlResponse result = apiInstance.MultiThreatScanUrlPost(body);
                Debug.WriteLine(result);
            }
            catch (ApiException  e)
            {
                Debug.Print("Exception when calling MultiThreatApi.MultiThreatScanUrlPost: " + e.Message);
                Debug.Print("Status Code: " + e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

#### Using the MultiThreatScanUrlPostWithHttpInfo variant
This returns an ApiResponse object which contains the response data, status code and headers.

```csharp
try
{
    // Scan a URL for multiple threat types including viruses, phishing, and policy violations in a single API call. Optionally download and scan the file at the URL.
    ApiResponse<MultiThreatUrlResponse> response = apiInstance.MultiThreatScanUrlPostWithHttpInfo(body);
    Debug.Write("Status Code: " + response.StatusCode);
    Debug.Write("Response Headers: " + response.Headers);
    Debug.Write("Response Body: " + response.Data);
}
catch (ApiException e)
{
    Debug.Print("Exception when calling MultiThreatApi.MultiThreatScanUrlPostWithHttpInfo: " + e.Message);
    Debug.Print("Status Code: " + e.ErrorCode);
    Debug.Print(e.StackTrace);
}
```

### Parameters

| Name | Type | Description | Notes |
|------|------|-------------|-------|
| **body** | [**MultiThreatUrlRequest**](MultiThreatUrlRequest.md) | URL scan request with URL and scan configuration | [optional]  |

### Return type

[**MultiThreatUrlResponse**](MultiThreatUrlResponse.md)

### Authorization

[Apikey](../README.md#Apikey)

### HTTP request headers

 - **Content-Type**: application/json, text/json, application/*+json
 - **Accept**: text/plain, application/json, text/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | OK |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

