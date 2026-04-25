# Cloudmersive.APIClient.NETCore.MultiThreatScan.Model.ContentScanningResult
Result of content scanning (downloading and scanning a file from URL)

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** | Whether content scanning was enabled | [optional] 
**DownloadedFileFormat** | **string** | Detected file format of downloaded content | [optional] 
**NsfwDetection** | [**NsfwDetectionResult**](NsfwDetectionResult.md) |  | [optional] 
**AiContentDetection** | [**AiContentDetectionResult**](AiContentDetectionResult.md) |  | [optional] 
**FraudDetection** | [**FraudDetectionResult**](FraudDetectionResult.md) |  | [optional] 
**SpamDetection** | [**SpamDetectionResult**](SpamDetectionResult.md) |  | [optional] 
**DlpDetection** | [**DlpDetectionResult**](DlpDetectionResult.md) |  | [optional] 
**PolicyEnforcement** | [**PolicyEnforcementResult**](PolicyEnforcementResult.md) |  | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

