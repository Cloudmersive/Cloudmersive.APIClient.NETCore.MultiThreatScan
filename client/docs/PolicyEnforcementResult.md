# Cloudmersive.APIClient.NETCore.MultiThreatScan.Model.PolicyEnforcementResult
Policy enforcement result

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | **bool** | Whether this scan was enabled | [optional] 
**Successful** | **bool** | Whether this scan completed successfully | [optional] 
**CleanResult** | **bool** | True if no policy violations were found | [optional] 
**RiskScore** | **double** | Overall risk score (0.0 to 1.0) | [optional] 
**RuleViolations** | [**List&lt;PolicyRuleViolation&gt;**](PolicyRuleViolation.md) | List of rule violations found | [optional] 
**Skipped** | **bool** | Scan was skipped | [optional] 
**SkipReason** | **string** | Reason the scan was skipped | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

