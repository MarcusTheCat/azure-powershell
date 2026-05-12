## 16.0.0 - June 2026
#### Az.Compute 11.6.0 
* Modified cmdlet `New-AzRestorePoint`
   - Added parameter `-InstantAccessDurationInMinutes`
* Modified cmdlet `New-AzRestorePointCollection`
   - Added parameter `-InstantAccess`
* Modified cmdlet `Update-AzRestorePointCollection`
   - Added parameter `-InstantAccess`
#### Az.LoadTesting 2.0.0 
* Modified cmdlet `New-AzLoad`
   - Removed parameters `-IdentityType`, `-IdentityUserAssigned`
   - Added parameters `-JsonFilePath`, `-JsonString`, `-EnableSystemAssignedIdentity`, `-UserAssignedIdentity`
* Modified cmdlet `Update-AzLoad`
   - Removed parameters `-IdentityType`, `-IdentityUserAssigned`
   - Added parameters `-JsonFilePath`, `-JsonString`, `-EnableSystemAssignedIdentity`, `-UserAssignedIdentity`
#### Az.Migrate 3.0.0 
* Modified cmdlet `Get-AzMigrateReplicationFabric`
   - Added parameter `-VaultInputObject`
* Modified cmdlet `Get-AzMigrateReplicationPolicy`
   - Added parameter `-VaultInputObject`
* Modified cmdlet `Get-AzMigrateReplicationProtectionContainer`
   - Added parameters `-ReplicationFabricInputObject`, `-VaultInputObject`
* Modified cmdlet `Get-AzMigrateReplicationProtectionContainerMapping`
   - Added parameters `-ReplicationFabricInputObject`, `-ReplicationProtectionContainerInputObject`, `-VaultInputObject`
* Modified cmdlet `Get-AzMigrateReplicationRecoveryServicesProvider`
   - Added parameters `-ReplicationFabricInputObject`, `-VaultInputObject`
* Modified cmdlet `Get-AzMigrateRunAsAccount`
   - Added parameters `-SubscriptionInputObject`, `-VMwareSiteInputObject`
* Modified cmdlet `Get-AzMigrateSite`
   - `SupportsShouldProcess` changed from False to True
   - Added parameters `-SubscriptionInputObject`, `-Subscription1InputObject`, `-Subscription2InputObject`
* Modified cmdlet `Get-AzMigrateSolution`
   - Added parameter `-MigrateProjectInputObject`
* Modified cmdlet `New-AzMigrateReplicationPolicy`
   - Added parameters `-JsonFilePath`, `-JsonString`
* Modified cmdlet `New-AzMigrateReplicationProtectionContainerMapping`
   - Added parameters `-JsonFilePath`, `-JsonString`
* Modified cmdlet `Register-AzMigrateProjectTool`
   - Added parameters `-JsonFilePath`, `-JsonString`
   - Output type changed from ``Boolean`` to ``IRegistrationResult``
#### Az.Monitor 8.0.0 
* Modified cmdlet `New-AzMonitorWorkspace`
   - Added parameters `-JsonFilePath`, `-JsonString`
* Modified cmdlet `New-AzPipelineGroup`
   - Removed parameter `-NetworkingConfiguration`
   - Added parameters `-DistributionMaxInstancesPerHost`, `-ExecutionPlacementConstraint`, `-TlsConfiguration`
* Modified cmdlet `Update-AzMonitorWorkspace`
   - Added parameters `-JsonFilePath`, `-JsonString`
* Modified cmdlet `Update-AzPipelineGroup`
   - Removed parameter `-NetworkingConfiguration`
   - Added parameters `-DistributionMaxInstancesPerHost`, `-ExecutionPlacementConstraint`, `-TlsConfiguration`
#### Az.Network 8.0.0 
* Modified cmdlet `New-AzFirewallPolicy`
   - Changed the type of parameter `-UserAssignedIdentityId` from `String` to `String[]`
* Modified cmdlet `Set-AzFirewallPolicy`
   - Changed the type of parameter `-UserAssignedIdentityId` from `String` to `String[]`
#### Az.PolicyInsights 2.0.0 
* Modified cmdlet `Get-AzPolicyAttestation`
   - Added parameters `-SubscriptionId`, `-InputObject`
   - Added parameter alias `AttestationName` to parameter `-Name`
   - Parameter `-Name` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Scope` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Removed parameter alias `Id` from parameter `-ResourceId`
   - Parameter `-ResourceId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Filter` ValidateNotNullOrEmpty changed from `True` to `False`
   - Output type changed from ``PSAttestation`` to ``IAttestation``
* Modified cmdlet `Get-AzPolicyEvent`
   - `SupportsShouldProcess` changed from False to True
   - Added parameter `-Expand`
   - Parameter `-ManagementGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Changed the type of parameter `-SubscriptionId` from `String` to `String[]`
   - Parameter `-SubscriptionId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicySetDefinitionName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicyDefinitionName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicyAssignmentName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-OrderBy` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Select` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Filter` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Apply` ValidateNotNullOrEmpty changed from `True` to `False`
   - Output type changed from ``PolicyEvent`` to ``IPolicyEvent``
* Modified cmdlet `Get-AzPolicyMetadata`
   - Added parameter alias `ResourceName` to parameter `-Name`
   - Parameter `-Name` ValidateNotNullOrEmpty changed from `True` to `False`
   - Output type changed from ``PSPolicyMetadata`` to ``IPolicyMetadata``
* Modified cmdlet `Get-AzPolicyRemediation`
   - Removed parameter `-ManagementGroupName`
   - Added parameters `-SubscriptionId`, `-ManagementGroupId`, `-InputObject`
   - Added parameter alias `RemediationName` to parameter `-Name`
   - Parameter `-Name` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Scope` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Removed parameter alias `Id` from parameter `-ResourceId`
   - Parameter `-ResourceId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Filter` ValidateNotNullOrEmpty changed from `True` to `False`
   - Output type changed from ``PSRemediation`` to ``IRemediation``
* Modified cmdlet `Get-AzPolicyState`
   - `SupportsShouldProcess` changed from False to True
   - Parameter `-ManagementGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Changed the type of parameter `-SubscriptionId` from `String` to `String[]`
   - Parameter `-SubscriptionId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicySetDefinitionName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicyDefinitionName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicyAssignmentName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-OrderBy` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Select` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Filter` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Apply` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Expand` ValidateNotNullOrEmpty changed from `True` to `False`
   - Output type changed from ``PolicyState`` to ``IPolicyState``
* Modified cmdlet `Get-AzPolicyStateSummary`
   - `SupportsShouldProcess` changed from False to True
   - Parameter `-ManagementGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-SubscriptionId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicySetDefinitionName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicyDefinitionName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicyAssignmentName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Filter` ValidateNotNullOrEmpty changed from `True` to `False`
   - Output type changed from ``PolicyStateSummary`` to ``ISummary``
* Modified cmdlet `New-AzPolicyAttestation`
   - Added parameters `-SubscriptionId`, `-InputObject`
   - Added parameter alias `AttestationName` to parameter `-Name`
   - Parameter `-Name` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicyAssignmentId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Changed the type of parameter `-ExpiresOn` from `Nullable`1[System.DateTime]` to `DateTime`
   - Changed the type of parameter `-Evidence` from `PSAttestationEvidence[]` to `IAttestationEvidence[]`
   - Changed the type of parameter `-AssessmentDate` from `Nullable`1[System.DateTime]` to `DateTime`
   - Output type changed from ``PSAttestation`` to ``IAttestation``
* Modified cmdlet `Remove-AzPolicyAttestation`
   - Added parameter `-SubscriptionId`
   - Added parameter alias `AttestationName` to parameter `-Name`
   - Parameter `-Name` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Scope` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Changed the type of parameter `-InputObject` from `PSAttestation` to `IPolicyInsightsIdentity`
* Modified cmdlet `Remove-AzPolicyRemediation`
   - Removed parameter `-ManagementGroupName`
   - Added parameters `-SubscriptionId`, `-ManagementGroupId`
   - Added parameter alias `RemediationName` to parameter `-Name`
   - Parameter `-Name` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Scope` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Removed parameter alias `Id` from parameter `-ResourceId`
   - Parameter `-ResourceId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Changed the type of parameter `-InputObject` from `PSRemediation` to `IPolicyInsightsIdentity`
* Removed cmdlet `Set-AzPolicyAttestation`
* Modified cmdlet `Start-AzPolicyComplianceScan`
   - Added parameters `-SubscriptionId`, `-NoWait`
   - Parameter `-ResourceGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
* Modified cmdlet `Start-AzPolicyRemediation`
   - Removed parameters `-ManagementGroupName`, `-LocationFilter`, `-ParallelDeploymentCount`, `-FailureThreshold`
   - Added parameters `-SubscriptionId`, `-ManagementGroupId`, `-InputObject`, `-FailureThresholdPercentage`, `-FilterLocation`, `-FilterResourceId`, `-ParallelDeployment`, `-NoWait`
   - Added parameter alias `RemediationName` to parameter `-Name`
   - Parameter `-Name` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Scope` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicyAssignmentId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-PolicyDefinitionReferenceId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Changed the type of parameter `-ResourceCount` from `Nullable`1[System.Int32]` to `Int32`
   - Output type changed from ``PSRemediation`` to ``IRemediation``
* Modified cmdlet `Stop-AzPolicyRemediation`
   - Removed parameters `-ManagementGroupName`, `-PassThru`
   - Added parameters `-SubscriptionId`, `-ManagementGroupId`, `-NoWait`
   - Added parameter alias `RemediationName` to parameter `-Name`
   - Parameter `-Name` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-Scope` ValidateNotNullOrEmpty changed from `True` to `False`
   - Parameter `-ResourceGroupName` ValidateNotNullOrEmpty changed from `True` to `False`
   - Removed parameter alias `Id` from parameter `-ResourceId`
   - Parameter `-ResourceId` ValidateNotNullOrEmpty changed from `True` to `False`
   - Changed the type of parameter `-InputObject` from `PSRemediation` to `IPolicyInsightsIdentity`
   - Output type changed from ``Boolean`` to ``IRemediation``
* Added cmdlet `Update-AzPolicyAttestation`
#### Az.ResourceMover 2.0.0 
* Modified cmdlet `Add-AzResourceMoverMoveResource`
   - Added parameters `-MoveCollectionInputObject`, `-JsonFilePath`, `-JsonString`
* Modified cmdlet `Get-AzResourceMoverMoveResource`
   - Added parameter `-MoveCollectionInputObject`
* Modified cmdlet `Get-AzResourceMoverUnresolvedDependency`
   - Changed the type of parameter `-DependencyLevel` from `DependencyLevel` to `String`
* Modified cmdlet `Invoke-AzResourceMoverBulkRemove`
   - Added parameters `-JsonFilePath`, `-JsonString`
   - Changed the type of parameter `-MoveResourceInputType` from `MoveResourceInputType` to `String`
* Modified cmdlet `Invoke-AzResourceMoverCommit`
   - Added parameters `-JsonFilePath`, `-JsonString`
   - Changed the type of parameter `-MoveResourceInputType` from `MoveResourceInputType` to `String`
* Modified cmdlet `Invoke-AzResourceMoverDiscard`
   - Added parameters `-JsonFilePath`, `-JsonString`
   - Changed the type of parameter `-MoveResourceInputType` from `MoveResourceInputType` to `String`
* Modified cmdlet `Invoke-AzResourceMoverInitiateMove`
   - Added parameters `-JsonFilePath`, `-JsonString`
   - Changed the type of parameter `-MoveResourceInputType` from `MoveResourceInputType` to `String`
* Modified cmdlet `Invoke-AzResourceMoverPrepare`
   - Added parameters `-JsonFilePath`, `-JsonString`
   - Changed the type of parameter `-MoveResourceInputType` from `MoveResourceInputType` to `String`
* Modified cmdlet `New-AzResourceMoverMoveCollection`
   - Removed parameter `-IdentityType`
   - Added parameters `-EnableSystemAssignedIdentity`, `-JsonFilePath`, `-JsonString`
   - Changed the type of parameter `-MoveType` from `MoveType` to `String`
* Modified cmdlet `Remove-AzResourceMoverMoveResource`
   - Added parameter `-MoveCollectionInputObject`
#### Az.ServiceFabric 5.2.0 
* Added cmdlet `Get-AzServiceFabricManagedClusterMaintenanceWindowStatus`
#### Az.Sql 6.5.0 
* Modified cmdlet `New-AzSqlSyncGroup`
   - Added parameters `-HubDatabaseAuthenticationType`, `-ResourceId`
* Modified cmdlet `New-AzSqlSyncMember`
   - Added parameters `-MemberDatabaseAuthenticationType`, `-ResourceId`
* Modified cmdlet `Update-AzSqlSyncGroup`
   - Added parameters `-HubDatabaseAuthenticationType`, `-ResourceId`, `-RemoveIdentityResourceId`
* Modified cmdlet `Update-AzSqlSyncMember`
   - Added parameters `-MemberDatabaseAuthenticationType`, `-ResourceId`, `-RemoveIdentityResourceId`


