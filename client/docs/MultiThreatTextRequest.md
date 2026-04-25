# Cloudmersive.APIClient.NETCore.MultiThreatScan.Model.MultiThreatTextRequest
Request to scan text for multiple threat types

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TextContent** | **string** | The text content to scan | [optional] 
**VirusScan** | [**VirusScanConfig**](VirusScanConfig.md) |  | [optional] 
**PhishingDetection** | [**PhishingDetectionTextConfig**](PhishingDetectionTextConfig.md) |  | [optional] 
**SpamDetection** | [**SpamDetectionConfig**](SpamDetectionConfig.md) |  | [optional] 
**DlpDetection** | [**DlpDetectionConfig**](DlpDetectionConfig.md) |  | [optional] 
**PolicyEnforcement** | [**PolicyEnforcementConfig**](PolicyEnforcementConfig.md) |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

