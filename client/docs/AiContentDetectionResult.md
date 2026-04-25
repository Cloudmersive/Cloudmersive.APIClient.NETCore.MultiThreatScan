# Cloudmersive.APIClient.NETCore.MultiThreatScan.Model.AiContentDetectionResult
AI content detection result

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** | Whether this scan was enabled | [optional] 
**Successful** | **bool** | Whether this scan completed successfully | [optional] 
**CleanResult** | **bool** | True if no AI-generated content was detected | [optional] 
**ContainsAiGeneratedContent** | **bool** | Content appears to be AI-generated | [optional] 
**AiConfidenceLevel** | **double** | Confidence level of AI content detection (0.0 to 1.0) | [optional] 
**Skipped** | **bool** | Scan was skipped | [optional] 
**SkipReason** | **string** | Reason the scan was skipped | [optional] 
**Verdict** | **string** | Categorical assessment of whether the file appears AI-generated based on its  embedded metadata. One of: NoDeterministicAiMetadataFound, VerifiedAiGenerated,  VerifiedAiEditedOrComposite, LikelyAiGenerated, LikelyAiEditedOrComposite,  PossibleAiGenerated, ConflictingSignals, MetadataUnavailableOrUnreadable,  UnsupportedFileType. | [optional] 
**Provider** | **string** | AI provider name (for example, \&quot;OpenAI\&quot;, \&quot;Adobe\&quot;, \&quot;Google\&quot;, \&quot;Microsoft\&quot;).  Empty when the metadata does not identify a provider. | [optional] 
**Generator** | **string** | AI tool or product name (for example, \&quot;ChatGPT\&quot;, \&quot;Adobe Firefly\&quot;, \&quot;Stable  Diffusion\&quot;). Empty when the metadata does not identify a specific tool. | [optional] 
**Warnings** | **List&lt;string&gt;** | Non-fatal warnings produced during analysis, intended for diagnostic display.  Empty when no warnings were produced. | [optional] 
**DetectedFileType** | **string** | File type detected from the file&#39;s content (for example, \&quot;jpeg\&quot;, \&quot;png\&quot;, \&quot;pdf\&quot;).  May differ from the file&#39;s name extension when the content was misnamed. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

