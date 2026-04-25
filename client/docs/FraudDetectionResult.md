# Cloudmersive.APIClient.NETCore.MultiThreatScan.Model.FraudDetectionResult
Fraud detection result

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** | Whether this scan was enabled | [optional] 
**Successful** | **bool** | Whether this scan completed successfully | [optional] 
**CleanResult** | **bool** | True if no fraud was detected | [optional] 
**FraudRiskLevel** | **double** | Fraud risk level (0.0 to 1.0) | [optional] 
**ContainsFinancialLiability** | **bool** | Document contains financial liability language | [optional] 
**ContainsSensitiveInformationCollection** | **bool** | Document collects sensitive information | [optional] 
**ContainsAssetTransfer** | **bool** | Document involves asset transfer | [optional] 
**ContainsPurchaseAgreement** | **bool** | Document is a purchase agreement | [optional] 
**ContainsEmploymentAgreement** | **bool** | Document is an employment agreement | [optional] 
**ContainsExpiredDocument** | **bool** | Document is expired | [optional] 
**ContainsAiGeneratedContent** | **bool** | Document contains AI-generated content | [optional] 
**AnalysisRationale** | **string** | Analysis rationale | [optional] 
**DocumentClass** | **string** | Document class/type | [optional] 
**Skipped** | **bool** | Scan was skipped | [optional] 
**SkipReason** | **string** | Reason the scan was skipped | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

