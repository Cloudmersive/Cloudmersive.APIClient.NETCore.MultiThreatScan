# Cloudmersive.APIClient.NETCore.MultiThreatScan.Model.PhishingDetectionTextResult
Phishing detection result for text scanning

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** | Whether this scan was enabled | [optional] 
**Successful** | **bool** | Whether this scan completed successfully | [optional] 
**CleanResult** | **bool** | True if no phishing was detected | [optional] 
**ContainsPhishing** | **bool** | Text contains phishing | [optional] 
**ContainsUnsolicitedSales** | **bool** | Text contains unsolicited sales | [optional] 
**ContainsPromotionalContent** | **bool** | Text contains promotional content | [optional] 
**ContainsWebUrls** | **bool** | Text contains web URLs | [optional] 
**ContainsPhoneNumbers** | **bool** | Text contains phone numbers | [optional] 
**ContainsEmailAddresses** | **bool** | Text contains email addresses | [optional] 
**ConfidenceLevel** | **double** | Confidence level (0.0 to 1.0) | [optional] 
**AnalysisRationale** | **string** | Analysis rationale | [optional] 
**UnsafeUrls** | [**List&lt;UnsafeUrlInfo&gt;**](UnsafeUrlInfo.md) | List of unsafe URLs found | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

