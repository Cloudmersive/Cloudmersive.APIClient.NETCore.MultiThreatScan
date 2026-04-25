# Cloudmersive.APIClient.NETCore.MultiThreatScan.Model.MultiThreatUrlRequest
Request to scan a URL for multiple threat types

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** | The URL to scan (must include http:// or https://) | [optional] 
**VirusScan** | [**UrlVirusScanConfig**](UrlVirusScanConfig.md) |  | [optional] 
**PhishingDetection** | [**UrlPhishingDetectionConfig**](UrlPhishingDetectionConfig.md) |  | [optional] 
**PolicyEnforcement** | [**PolicyEnforcementConfig**](PolicyEnforcementConfig.md) |  | [optional] 
**ContentScanning** | [**ContentScanningConfig**](ContentScanningConfig.md) |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

