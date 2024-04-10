# Comparing `tmp/cudo_compute-0.1.7.tar.gz` & `tmp/cudo_compute-0.1.8.tar.gz`

## Comparing `cudo_compute-0.1.7.tar` & `cudo_compute-0.1.8.tar`

### file list

```diff
@@ -1,1064 +1,1069 @@
--rwxr-xr-x   0        0        0      685 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/codegen.sh
--rw-r--r--   0        0        0   179513 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/fix.swagger.json
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/.github/workflows/workflow-test.yml
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/.github/workflows/workflow.yml
--rw-r--r--   0        0        0    27365 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/README.md
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/APIKeysApi.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ActivateBody.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/AddBillingAccountUserPermissionBody.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/AddDataCenterUserPermissionBody.md
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/AddProjectUserPermissionBody.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Any.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ApiKey.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/AttachSecurityGroupResponse.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/AttachStorageDiskResponse.md
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/BillingAccount.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/BillingAccountPaymentMethod.md
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/BillingAccountPaymentMethods.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/BillingAccountSetupIntent.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/BillingAccountSpendRow.md
--rw-r--r--   0        0        0    19349 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/BillingApi.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Cluster.md
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ConnectVMResponse.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CountHostsResponse.md
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CountVMsResponse.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CpuModelCategory.md
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateBillingAccountRequest.md
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateDiskSnapshotBody.md
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateDiskSnapshotResponse.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateNetworkBody.md
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateNetworkResponse.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateObjectStorageUserBody.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreatePrivateVMImageResponse.md
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateSecurityGroupResponse.md
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateStorageDiskBody.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateStorageDiskResponse.md
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateVMBody.md
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateVMRequestNIC.md
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/CreateVMResponse.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DataCenter.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DataCenterCategory.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DataCenterRevenueResource.md
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DataCenterTimeRevenue.md
--rw-r--r--   0        0        0    15819 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DataCentersApi.md
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Decimal.md
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DeleteDiskSnapshotResponse.md
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DeleteNetworkResponse.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DeleteObjectStorageKeyResponse.md
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DeleteObjectStorageUserResponse.md
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DeletePrivateVMImageResponse.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DeleteSecurityGroupResponse.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DeleteStorageDiskResponse.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DetachSecurityGroupResponse.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DetachStorageDiskResponse.md
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Disk.md
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DiskState.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DiskStorageClass.md
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DiskStoragePriceHr.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DiskType.md
--rw-r--r--   0        0        0    14900 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/DisksApi.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GenerateApiKeyRequest.md
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetBillingAccountDetailsResponse.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetBillingAccountSpendDetailsResponse.md
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetBillingAccountStripeInvoicesResponse.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetDataCenterLiveUtilizationResponse.md
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetDataCenterRevenueByResourceResponse.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetDataCenterRevenueTimeSeriesResponse.md
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetDiskResponse.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetMachineTypeLiveUtilizationResponse.md
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetMachineTypeResponse.md
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetNetworkResponse.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetObjectStorageSessionKeyResponse.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetPrivateVMImageResponse.md
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetSecurityGroupResponse.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GetVMResponse.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/GpuModelCategory.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Host.md
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/HostConfigCategory.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/IdentityVerificationSession.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Image.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Interval.md
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Invoice.md
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListApiKeysResponse.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListBillingAccountsResponse.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListClustersResponse.md
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListDataCentersResponse.md
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListDiskSnapshotsResponse.md
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListDisksResponse.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListHostsResponse.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListMachineTypesResponse.md
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListNetworksResponse.md
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListObjectStorageBucketsResponse.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListObjectStorageKeysResponse.md
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListObjectStorageUsersResponse.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListOutstandingStripeInvoicesResponse.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListPrivateVMImagesResponse.md
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListPrivateVMImagesResponsePrivateImage.md
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListProjectSshKeysResponse.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListProjectsResponse.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListPublicVMImagesResponse.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListRegionsResponse.md
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListSecurityGroupsResponse.md
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListSshKeysResponse.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListUserPermissionsResponse.md
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListVMDataCentersResponse.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListVMDisksResponse.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListVMMachineTypesRequest.md
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListVMMachineTypesResponse.md
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ListVMsResponse.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/MachineType.md
--rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/MachineTypesApi.md
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/MonitorVMResponse.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Network.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/NetworkPriceHr.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/NetworkState.md
--rw-r--r--   0        0        0    16589 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/NetworksApi.md
--rw-r--r--   0        0        0    16273 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ObjectStorageApi.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ObjectStorageBucket.md
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ObjectStorageKey.md
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ObjectStorageUser.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/PaymentMethodCard.md
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/PaymentMethodPaypal.md
--rw-r--r--   0        0        0    12202 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/PermissionsApi.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Point.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Profile.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Project.md
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ProjectsApi.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Protocol.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/RebootVMResponse.md
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Region.md
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/RemoveBillingAccountPaymentMethodResponse.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/RemoveBillingAccountUserPermissionBody.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/RemoveDataCenterUserPermissionBody.md
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/RemoveProjectUserPermissionBody.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ResizeVMDiskResponse.md
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/ResizeVMResponse.md
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/RevertDiskResponse.md
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Role.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Rule.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/RuleType.md
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/SSHKeysApi.md
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/SearchApi.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/SecurityGroup.md
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/SecurityGroup1.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/SecurityGroupRule.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/SetBillingAccountDefaultPaymentMethodResponse.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Snapshot.md
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/SshKey.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/SshKeySource.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/StartNetworkResponse.md
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/StartVMResponse.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Status.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/StopNetworkResponse.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/StopVMResponse.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/StripeCustomer.md
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/TaxId.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/TerminateVMResponse.md
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/Unit.md
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/UpdateBillingAccountBody.md
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/UpdatePrivateVMImageResponse.md
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/UpdateSecurityGroupResponse.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/UpdateVMMetadataBody.md
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/UpdateVMMetadataResponse.md
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/UserApi.md
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/UserPermission.md
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/V1PrivateImage.md
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/V1billingaccountsbillingAccountIdBillingAccount.md
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/VM.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/VMDataCenter.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/VMDataCenterStorageClass.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/VMMonitoringItem.md
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/VMNIC.md
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/VRouterSize.md
--rw-r--r--   0        0        0    35782 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/VirtualMachinesApi.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/docs/VmState.md
--rw-r--r--   0        0        0    13838 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/__init__.py
--rw-r--r--   0        0        0    25116 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api_client.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/auth_config.py
--rw-r--r--   0        0        0     8056 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/configuration.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/cudo_api.py
--rw-r--r--   0        0        0    13204 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/rest.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/__init__.py
--rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/api_keys_api.py
--rw-r--r--   0        0        0    55650 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/billing_api.py
--rw-r--r--   0        0        0    48150 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/data_centers_api.py
--rw-r--r--   0        0        0    48678 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/disks_api.py
--rw-r--r--   0        0        0    14135 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/machine_types_api.py
--rw-r--r--   0        0        0    52886 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/networks_api.py
--rw-r--r--   0        0        0    47393 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/object_storage_api.py
--rw-r--r--   0        0        0    35510 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/permissions_api.py
--rw-r--r--   0        0        0    23476 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/projects_api.py
--rw-r--r--   0        0        0     3938 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/search_api.py
--rw-r--r--   0        0        0    15229 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/ssh_keys_api.py
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/user_api.py
--rw-r--r--   0        0        0   108046 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/api/virtual_machines_api.py
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/__init__.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/activate_body.py
--rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/add_billing_account_user_permission_body.py
--rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/add_data_center_user_permission_body.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/add_project_user_permission_body.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/any.py
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/api_key.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/attach_security_group_response.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/attach_storage_disk_response.py
--rw-r--r--   0        0        0    10794 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/billing_account.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/billing_account_payment_method.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/billing_account_payment_methods.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/billing_account_setup_intent.py
--rw-r--r--   0        0        0     7856 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/billing_account_spend_row.py
--rw-r--r--   0        0        0    23207 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/cluster.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/connect_vm_response.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/count_hosts_response.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/count_vms_response.py
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/cpu_model_category.py
--rw-r--r--   0        0        0     6915 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_billing_account_request.py
--rw-r--r--   0        0        0     4457 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_disk_snapshot_body.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_disk_snapshot_response.py
--rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_network_body.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_network_response.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_object_storage_user_body.py
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_private_vm_image_response.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_security_group_response.py
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_storage_disk_body.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_storage_disk_response.py
--rw-r--r--   0        0        0    16675 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_vm_body.py
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_vm_request_nic.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/create_vm_response.py
--rw-r--r--   0        0        0     7194 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/data_center.py
--rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/data_center_category.py
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/data_center_revenue_resource.py
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/data_center_time_revenue.py
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/decimal.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_disk_snapshot_response.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_network_response.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_object_storage_key_response.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_object_storage_user_response.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_private_vm_image_response.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_security_group_response.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_storage_disk_response.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/detach_security_group_response.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/detach_storage_disk_response.py
--rw-r--r--   0        0        0    10418 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/disk.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/disk_state.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/disk_storage_class.py
--rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/disk_storage_price_hr.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/disk_type.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/generate_api_key_request.py
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_billing_account_details_response.py
--rw-r--r--   0        0        0     3775 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_billing_account_spend_details_response.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_billing_account_stripe_invoices_response.py
--rw-r--r--   0        0        0    15541 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_data_center_live_utilization_response.py
--rw-r--r--   0        0        0     3877 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_data_center_revenue_by_resource_response.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_data_center_revenue_time_series_response.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_disk_response.py
--rw-r--r--   0        0        0    15598 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_machine_type_live_utilization_response.py
--rw-r--r--   0        0        0    21097 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_machine_type_response.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_network_response.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_object_storage_session_key_response.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_private_vm_image_response.py
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_security_group_response.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/get_vm_response.py
--rw-r--r--   0        0        0     5406 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/gpu_model_category.py
--rw-r--r--   0        0        0    14801 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/host.py
--rw-r--r--   0        0        0    19136 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/host_config_category.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/identity_verification_session.py
--rw-r--r--   0        0        0     7225 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/image.py
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/interval.py
--rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/invoice.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_api_keys_response.py
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_billing_accounts_response.py
--rw-r--r--   0        0        0     3640 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_clusters_response.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_data_centers_response.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_disk_snapshots_response.py
--rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_disks_response.py
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_hosts_response.py
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_machine_types_response.py
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_networks_response.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_object_storage_buckets_response.py
--rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_object_storage_keys_response.py
--rw-r--r--   0        0        0     6430 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_object_storage_users_response.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_outstanding_stripe_invoices_response.py
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_private_vm_images_response.py
--rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_private_vm_images_response_private_image.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_project_ssh_keys_response.py
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_projects_response.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_public_vm_images_response.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_regions_response.py
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_security_groups_response.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_ssh_keys_response.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_user_permissions_response.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_vm_data_centers_response.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_vm_disks_response.py
--rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_vm_machine_types_request.py
--rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_vm_machine_types_response.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/list_vms_response.py
--rw-r--r--   0        0        0     7405 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/machine_type.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/monitor_vm_response.py
--rw-r--r--   0        0        0    11037 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/network.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/network_price_hr.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/network_state.py
--rw-r--r--   0        0        0     7851 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/object_storage_bucket.py
--rw-r--r--   0        0        0     6183 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/object_storage_key.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/object_storage_user.py
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/payment_method_card.py
--rw-r--r--   0        0        0     4210 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/payment_method_paypal.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/point.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/profile.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/project.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/protocol.py
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/reboot_vm_response.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/region.py
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/remove_billing_account_payment_method_response.py
--rw-r--r--   0        0        0     6243 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/remove_billing_account_user_permission_body.py
--rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/remove_data_center_user_permission_body.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/remove_project_user_permission_body.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/resize_vm_disk_response.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/resize_vm_response.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/revert_disk_response.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/role.py
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/rule.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/rule_type.py
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/security_group.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/security_group1.py
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/security_group_rule.py
--rw-r--r--   0        0        0     4819 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/set_billing_account_default_payment_method_response.py
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/snapshot.py
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/ssh_key.py
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/ssh_key_source.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/start_network_response.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/start_vm_response.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/status.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/stop_network_response.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/stop_vm_response.py
--rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/stripe_customer.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/tax_id.py
--rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/terminate_vm_response.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/unit.py
--rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/update_billing_account_body.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/update_private_vm_image_response.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/update_security_group_response.py
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/update_vm_metadata_body.py
--rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/update_vm_metadata_response.py
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/user_permission.py
--rw-r--r--   0        0        0     6178 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/v1_private_image.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/v_router_size.py
--rw-r--r--   0        0        0    25898 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/vm.py
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/vm_data_center.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/vm_data_center_storage_class.py
--rw-r--r--   0        0        0     8980 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/vm_monitoring_item.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/vm_state.py
--rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/docs/src/cudo_compute/models/vmnic.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/examples/example.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/helpers/auth_config.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/helpers/cudo_api.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/.gitignore
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/.swagger-codegen-ignore
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/.travis.yml
--rw-r--r--   0        0        0    27337 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/README.md
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/git_push.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/requirements.txt
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/setup.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test-requirements.txt
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/tox.ini
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/.swagger-codegen/VERSION
--rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/__init__.py
--rw-r--r--   0        0        0    25101 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api_client.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/configuration.py
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/rest.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/__init__.py
--rw-r--r--   0        0        0    12788 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/api_keys_api.py
--rw-r--r--   0        0        0    55647 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/billing_api.py
--rw-r--r--   0        0        0    48147 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/data_centers_api.py
--rw-r--r--   0        0        0    48675 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/disks_api.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/machine_types_api.py
--rw-r--r--   0        0        0    52883 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/networks_api.py
--rw-r--r--   0        0        0    47390 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/object_storage_api.py
--rw-r--r--   0        0        0    35507 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/permissions_api.py
--rw-r--r--   0        0        0    23473 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/projects_api.py
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/search_api.py
--rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/ssh_keys_api.py
--rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/user_api.py
--rw-r--r--   0        0        0   108043 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/api/virtual_machines_api.py
--rw-r--r--   0        0        0    12278 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/activate_body.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/add_billing_account_user_permission_body.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/add_data_center_user_permission_body.py
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/add_project_user_permission_body.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/any.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/api_key.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/attach_security_group_response.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/attach_storage_disk_response.py
--rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/billing_account.py
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/billing_account_payment_method.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/billing_account_payment_methods.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/billing_account_setup_intent.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/billing_account_spend_row.py
--rw-r--r--   0        0        0    23204 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/cluster.py
--rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/connect_vm_response.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/count_hosts_response.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/count_vms_response.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/cpu_model_category.py
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_billing_account_request.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_disk_snapshot_body.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_disk_snapshot_response.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_network_body.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_network_response.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_object_storage_user_body.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_private_vm_image_response.py
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_security_group_response.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_storage_disk_body.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_storage_disk_response.py
--rw-r--r--   0        0        0    16672 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_vm_body.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_vm_request_nic.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/create_vm_response.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/data_center.py
--rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/data_center_category.py
--rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/data_center_revenue_resource.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/data_center_time_revenue.py
--rw-r--r--   0        0        0     8588 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/decimal.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/delete_disk_snapshot_response.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/delete_network_response.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/delete_object_storage_key_response.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/delete_object_storage_user_response.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/delete_private_vm_image_response.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/delete_security_group_response.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/delete_storage_disk_response.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/detach_security_group_response.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/detach_storage_disk_response.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/disk.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/disk_state.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/disk_storage_class.py
--rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/disk_storage_price_hr.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/disk_type.py
--rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/generate_api_key_request.py
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_billing_account_details_response.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_billing_account_spend_details_response.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_billing_account_stripe_invoices_response.py
--rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_data_center_live_utilization_response.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_data_center_revenue_by_resource_response.py
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_data_center_revenue_time_series_response.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_disk_response.py
--rw-r--r--   0        0        0    15595 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_machine_type_live_utilization_response.py
--rw-r--r--   0        0        0    21094 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_machine_type_response.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_network_response.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_object_storage_session_key_response.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_private_vm_image_response.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_security_group_response.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/get_vm_response.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/gpu_model_category.py
--rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/host.py
--rw-r--r--   0        0        0    19133 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/host_config_category.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/identity_verification_session.py
--rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/image.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/interval.py
--rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/invoice.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_api_keys_response.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_billing_accounts_response.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_clusters_response.py
--rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_data_centers_response.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_disk_snapshots_response.py
--rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_disks_response.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_hosts_response.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_machine_types_response.py
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_networks_response.py
--rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_object_storage_buckets_response.py
--rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_object_storage_keys_response.py
--rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_object_storage_users_response.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_outstanding_stripe_invoices_response.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_private_vm_images_response.py
--rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_private_vm_images_response_private_image.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_project_ssh_keys_response.py
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_projects_response.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_public_vm_images_response.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_regions_response.py
--rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_security_groups_response.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_ssh_keys_response.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_user_permissions_response.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_vm_data_centers_response.py
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_vm_disks_response.py
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_vm_machine_types_request.py
--rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_vm_machine_types_response.py
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/list_vms_response.py
--rw-r--r--   0        0        0     7402 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/machine_type.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/monitor_vm_response.py
--rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/network.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/network_price_hr.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/network_state.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/object_storage_bucket.py
--rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/object_storage_key.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/object_storage_user.py
--rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/payment_method_card.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/payment_method_paypal.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/point.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/profile.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/project.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/protocol.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/reboot_vm_response.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/region.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/remove_billing_account_payment_method_response.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/remove_billing_account_user_permission_body.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/remove_data_center_user_permission_body.py
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/remove_project_user_permission_body.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/resize_vm_disk_response.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/resize_vm_response.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/revert_disk_response.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/role.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/rule.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/rule_type.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/security_group.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/security_group1.py
--rw-r--r--   0        0        0     6817 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/security_group_rule.py
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/set_billing_account_default_payment_method_response.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/snapshot.py
--rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/ssh_key.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/ssh_key_source.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/start_network_response.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/start_vm_response.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/status.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/stop_network_response.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/stop_vm_response.py
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/stripe_customer.py
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/tax_id.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/terminate_vm_response.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/unit.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/update_billing_account_body.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/update_private_vm_image_response.py
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/update_security_group_response.py
--rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/update_vm_metadata_body.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/update_vm_metadata_response.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/user_permission.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/v1_private_image.py
--rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/v_router_size.py
--rw-r--r--   0        0        0    25895 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/vm.py
--rw-r--r--   0        0        0     8588 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/vm_data_center.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/vm_data_center_storage_class.py
--rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/vm_monitoring_item.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/vm_state.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/cudo_compute/models/vmnic.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/APIKeysApi.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ActivateBody.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/AddBillingAccountUserPermissionBody.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/AddDataCenterUserPermissionBody.md
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/AddProjectUserPermissionBody.md
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Any.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ApiKey.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/AttachSecurityGroupResponse.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/AttachStorageDiskResponse.md
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/BillingAccount.md
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/BillingAccountPaymentMethod.md
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/BillingAccountPaymentMethods.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/BillingAccountSetupIntent.md
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/BillingAccountSpendRow.md
--rw-r--r--   0        0        0    19181 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/BillingApi.md
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Cluster.md
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ConnectVMResponse.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CountHostsResponse.md
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CountVMsResponse.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CpuModelCategory.md
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateBillingAccountRequest.md
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateDiskSnapshotBody.md
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateDiskSnapshotResponse.md
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateNetworkBody.md
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateNetworkResponse.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateObjectStorageUserBody.md
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreatePrivateVMImageResponse.md
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateSecurityGroupResponse.md
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateStorageDiskBody.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateStorageDiskResponse.md
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateVMBody.md
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateVMRequestNIC.md
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/CreateVMResponse.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DataCenter.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DataCenterCategory.md
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DataCenterRevenueResource.md
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DataCenterTimeRevenue.md
--rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DataCentersApi.md
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Decimal.md
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DeleteDiskSnapshotResponse.md
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DeleteNetworkResponse.md
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DeleteObjectStorageKeyResponse.md
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DeleteObjectStorageUserResponse.md
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DeletePrivateVMImageResponse.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DeleteSecurityGroupResponse.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DeleteStorageDiskResponse.md
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DetachSecurityGroupResponse.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DetachStorageDiskResponse.md
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Disk.md
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DiskState.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DiskStorageClass.md
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DiskStoragePriceHr.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DiskType.md
--rw-r--r--   0        0        0    14768 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/DisksApi.md
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GenerateApiKeyRequest.md
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetBillingAccountDetailsResponse.md
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetBillingAccountSpendDetailsResponse.md
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetBillingAccountStripeInvoicesResponse.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetDataCenterLiveUtilizationResponse.md
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetDataCenterRevenueByResourceResponse.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetDataCenterRevenueTimeSeriesResponse.md
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetDiskResponse.md
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetMachineTypeLiveUtilizationResponse.md
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetMachineTypeResponse.md
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetNetworkResponse.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetObjectStorageSessionKeyResponse.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetPrivateVMImageResponse.md
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetSecurityGroupResponse.md
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GetVMResponse.md
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/GpuModelCategory.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Host.md
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/HostConfigCategory.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/IdentityVerificationSession.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Image.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Interval.md
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Invoice.md
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListApiKeysResponse.md
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListBillingAccountsResponse.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListClustersResponse.md
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListDataCentersResponse.md
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListDiskSnapshotsResponse.md
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListDisksResponse.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListHostsResponse.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListMachineTypesResponse.md
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListNetworksResponse.md
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListObjectStorageBucketsResponse.md
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListObjectStorageKeysResponse.md
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListObjectStorageUsersResponse.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListOutstandingStripeInvoicesResponse.md
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListPrivateVMImagesResponse.md
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListPrivateVMImagesResponsePrivateImage.md
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListProjectSshKeysResponse.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListProjectsResponse.md
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListPublicVMImagesResponse.md
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListRegionsResponse.md
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListSecurityGroupsResponse.md
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListSshKeysResponse.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListUserPermissionsResponse.md
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListVMDataCentersResponse.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListVMDisksResponse.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListVMMachineTypesRequest.md
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListVMMachineTypesResponse.md
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ListVMsResponse.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/MachineType.md
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/MachineTypesApi.md
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/MonitorVMResponse.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Network.md
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/NetworkPriceHr.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/NetworkState.md
--rw-r--r--   0        0        0    16441 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/NetworksApi.md
--rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ObjectStorageApi.md
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ObjectStorageBucket.md
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ObjectStorageKey.md
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ObjectStorageUser.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/PaymentMethodCard.md
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/PaymentMethodPaypal.md
--rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/PermissionsApi.md
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Point.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Profile.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Project.md
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ProjectsApi.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Protocol.md
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/RebootVMResponse.md
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Region.md
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/RemoveBillingAccountPaymentMethodResponse.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/RemoveBillingAccountUserPermissionBody.md
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/RemoveDataCenterUserPermissionBody.md
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/RemoveProjectUserPermissionBody.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ResizeVMDiskResponse.md
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/ResizeVMResponse.md
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/RevertDiskResponse.md
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Role.md
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Rule.md
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/RuleType.md
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/SSHKeysApi.md
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/SearchApi.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/SecurityGroup.md
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/SecurityGroup1.md
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/SecurityGroupRule.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/SetBillingAccountDefaultPaymentMethodResponse.md
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Snapshot.md
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/SshKey.md
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/SshKeySource.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/StartNetworkResponse.md
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/StartVMResponse.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Status.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/StopNetworkResponse.md
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/StopVMResponse.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/StripeCustomer.md
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/TaxId.md
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/TerminateVMResponse.md
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/Unit.md
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/UpdateBillingAccountBody.md
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/UpdatePrivateVMImageResponse.md
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/UpdateSecurityGroupResponse.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/UpdateVMMetadataBody.md
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/UpdateVMMetadataResponse.md
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/UserApi.md
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/UserPermission.md
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/V1PrivateImage.md
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/V1billingaccountsbillingAccountIdBillingAccount.md
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/VM.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/VMDataCenter.md
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/VMDataCenterStorageClass.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/VMMonitoringItem.md
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/VMNIC.md
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/VRouterSize.md
--rw-r--r--   0        0        0    35482 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/VirtualMachinesApi.md
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/docs/VmState.md
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/__init__.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_activate_body.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_add_billing_account_user_permission_body.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_add_data_center_user_permission_body.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_add_project_user_permission_body.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_any.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_api_key.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_api_keys_api.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_attach_security_group_response.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_attach_storage_disk_response.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_billing_account.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_billing_account_payment_method.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_billing_account_payment_methods.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_billing_account_setup_intent.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_billing_account_spend_row.py
--rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_billing_api.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_cluster.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_connect_vm_response.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_count_hosts_response.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_count_vms_response.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_cpu_model_category.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_billing_account_request.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_disk_snapshot_body.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_disk_snapshot_response.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_network_body.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_network_response.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_object_storage_user_body.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_private_vm_image_response.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_security_group_response.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_storage_disk_body.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_storage_disk_response.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_vm_body.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_vm_request_nic.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_create_vm_response.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_data_center.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_data_center_category.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_data_center_revenue_resource.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_data_center_time_revenue.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_data_centers_api.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_decimal.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_delete_disk_snapshot_response.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_delete_network_response.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_delete_object_storage_key_response.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_delete_object_storage_user_response.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_delete_private_vm_image_response.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_delete_security_group_response.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_delete_storage_disk_response.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_detach_security_group_response.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_detach_storage_disk_response.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_disk.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_disk_state.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_disk_storage_class.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_disk_storage_price_hr.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_disk_type.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_disks_api.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_generate_api_key_request.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_billing_account_details_response.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_billing_account_spend_details_response.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_billing_account_stripe_invoices_response.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_data_center_live_utilization_response.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_data_center_revenue_by_resource_response.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_data_center_revenue_time_series_response.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_disk_response.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_machine_type_live_utilization_response.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_machine_type_response.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_network_response.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_object_storage_session_key_response.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_private_vm_image_response.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_security_group_response.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_get_vm_response.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_gpu_model_category.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_host.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_host_config_category.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_identity_verification_session.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_image.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_interval.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_invoice.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_api_keys_response.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_billing_accounts_response.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_clusters_response.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_data_centers_response.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_disk_snapshots_response.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_disks_response.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_hosts_response.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_machine_types_response.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_networks_response.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_object_storage_buckets_response.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_object_storage_keys_response.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_object_storage_users_response.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_outstanding_stripe_invoices_response.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_private_vm_images_response.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_private_vm_images_response_private_image.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_project_ssh_keys_response.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_projects_response.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_public_vm_images_response.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_regions_response.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_security_groups_response.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_ssh_keys_response.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_user_permissions_response.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_vm_data_centers_response.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_vm_disks_response.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_vm_machine_types_request.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_vm_machine_types_response.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_list_vms_response.py
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_machine_type.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_machine_types_api.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_monitor_vm_response.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_network.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_network_price_hr.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_network_state.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_networks_api.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_object_storage_api.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_object_storage_bucket.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_object_storage_key.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_object_storage_user.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_payment_method_card.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_payment_method_paypal.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_permissions_api.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_point.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_profile.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_project.py
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_projects_api.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_protocol.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_reboot_vm_response.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_region.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_remove_billing_account_payment_method_response.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_remove_billing_account_user_permission_body.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_remove_data_center_user_permission_body.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_remove_project_user_permission_body.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_resize_vm_disk_response.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_resize_vm_response.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_revert_disk_response.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_role.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_rule.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_rule_type.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_search_api.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_security_group.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_security_group1.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_security_group_rule.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_set_billing_account_default_payment_method_response.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_snapshot.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_ssh_key.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_ssh_key_source.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_ssh_keys_api.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_start_network_response.py
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_start_vm_response.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_status.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_stop_network_response.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_stop_vm_response.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_stripe_customer.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_tax_id.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_terminate_vm_response.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_unit.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_update_billing_account_body.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_update_private_vm_image_response.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_update_security_group_response.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_update_vm_metadata_body.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_update_vm_metadata_response.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_user_api.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_user_permission.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_v1_private_image.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_v1billingaccountsbilling_account_id_billing_account.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_v_router_size.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_virtual_machines_api.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_vm.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_vm_data_center.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_vm_data_center_storage_class.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_vm_monitoring_item.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_vm_state.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/out/test/test_vmnic.py
--rw-r--r--   0        0        0    13242 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/__init__.py
--rw-r--r--   0        0        0    25101 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api_client.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/auth_config.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/configuration.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/cudo_api.py
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/rest.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/__init__.py
--rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/api_keys_api.py
--rw-r--r--   0        0        0    55660 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/billing_api.py
--rw-r--r--   0        0        0    48158 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/data_centers_api.py
--rw-r--r--   0        0        0    48685 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/disks_api.py
--rw-r--r--   0        0        0    14135 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/machine_types_api.py
--rw-r--r--   0        0        0    52894 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/networks_api.py
--rw-r--r--   0        0        0    47400 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/object_storage_api.py
--rw-r--r--   0        0        0    35514 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/permissions_api.py
--rw-r--r--   0        0        0    23479 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/projects_api.py
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/search_api.py
--rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/ssh_keys_api.py
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/user_api.py
--rw-r--r--   0        0        0   108067 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/api/virtual_machines_api.py
--rw-r--r--   0        0        0    12278 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/__init__.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/activate_body.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/add_billing_account_user_permission_body.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/add_data_center_user_permission_body.py
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/add_project_user_permission_body.py
--rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/any.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/api_key.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/attach_security_group_response.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/attach_storage_disk_response.py
--rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/billing_account.py
--rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/billing_account_payment_method.py
--rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/billing_account_payment_methods.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/billing_account_setup_intent.py
--rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/billing_account_spend_row.py
--rw-r--r--   0        0        0    23204 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/cluster.py
--rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/connect_vm_response.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/count_hosts_response.py
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/count_vms_response.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/cpu_model_category.py
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_billing_account_request.py
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_disk_snapshot_body.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_disk_snapshot_response.py
--rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_network_body.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_network_response.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_object_storage_user_body.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_private_vm_image_response.py
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_security_group_response.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_storage_disk_body.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_storage_disk_response.py
--rw-r--r--   0        0        0    16672 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_vm_body.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_vm_request_nic.py
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/create_vm_response.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/data_center.py
--rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/data_center_category.py
--rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/data_center_revenue_resource.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/data_center_time_revenue.py
--rw-r--r--   0        0        0     8588 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/decimal.py
--rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/delete_disk_snapshot_response.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/delete_network_response.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/delete_object_storage_key_response.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/delete_object_storage_user_response.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/delete_private_vm_image_response.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/delete_security_group_response.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/delete_storage_disk_response.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/detach_security_group_response.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/detach_storage_disk_response.py
--rw-r--r--   0        0        0    10415 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/disk.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/disk_state.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/disk_storage_class.py
--rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/disk_storage_price_hr.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/disk_type.py
--rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/generate_api_key_request.py
--rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_billing_account_details_response.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_billing_account_spend_details_response.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_billing_account_stripe_invoices_response.py
--rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_data_center_live_utilization_response.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_data_center_revenue_by_resource_response.py
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_data_center_revenue_time_series_response.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_disk_response.py
--rw-r--r--   0        0        0    15595 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_machine_type_live_utilization_response.py
--rw-r--r--   0        0        0    21094 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_machine_type_response.py
--rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_network_response.py
--rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_object_storage_session_key_response.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_private_vm_image_response.py
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_security_group_response.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/get_vm_response.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/gpu_model_category.py
--rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/host.py
--rw-r--r--   0        0        0    19133 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/host_config_category.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/identity_verification_session.py
--rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/image.py
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/interval.py
--rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/invoice.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_api_keys_response.py
--rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_billing_accounts_response.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_clusters_response.py
--rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_data_centers_response.py
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_disk_snapshots_response.py
--rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_disks_response.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_hosts_response.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_machine_types_response.py
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_networks_response.py
--rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_object_storage_buckets_response.py
--rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_object_storage_keys_response.py
--rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_object_storage_users_response.py
--rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_outstanding_stripe_invoices_response.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_private_vm_images_response.py
--rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_private_vm_images_response_private_image.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_project_ssh_keys_response.py
--rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_projects_response.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_public_vm_images_response.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_regions_response.py
--rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_security_groups_response.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_ssh_keys_response.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_user_permissions_response.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_vm_data_centers_response.py
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_vm_disks_response.py
--rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_vm_machine_types_request.py
--rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_vm_machine_types_response.py
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/list_vms_response.py
--rw-r--r--   0        0        0     7402 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/machine_type.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/monitor_vm_response.py
--rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/network.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/network_price_hr.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/network_state.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/object_storage_bucket.py
--rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/object_storage_key.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/object_storage_user.py
--rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/payment_method_card.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/payment_method_paypal.py
--rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/point.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/profile.py
--rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/project.py
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/protocol.py
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/reboot_vm_response.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/region.py
--rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/remove_billing_account_payment_method_response.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/remove_billing_account_user_permission_body.py
--rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/remove_data_center_user_permission_body.py
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/remove_project_user_permission_body.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/resize_vm_disk_response.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/resize_vm_response.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/revert_disk_response.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/role.py
--rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/rule.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/rule_type.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/security_group.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/security_group1.py
--rw-r--r--   0        0        0     6817 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/security_group_rule.py
--rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/set_billing_account_default_payment_method_response.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/snapshot.py
--rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/ssh_key.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/ssh_key_source.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/start_network_response.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/start_vm_response.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/status.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/stop_network_response.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/stop_vm_response.py
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/stripe_customer.py
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/tax_id.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/terminate_vm_response.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/unit.py
--rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/update_billing_account_body.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/update_private_vm_image_response.py
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/update_security_group_response.py
--rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/update_vm_metadata_body.py
--rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/update_vm_metadata_response.py
--rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/user_permission.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/v1_private_image.py
--rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/v_router_size.py
--rw-r--r--   0        0        0    25895 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/vm.py
--rw-r--r--   0        0        0     8588 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/vm_data_center.py
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/vm_data_center_storage_class.py
--rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/vm_monitoring_item.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/vm_state.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/src/cudo_compute/models/vmnic.py
--rw-r--r--   0        0        0   179189 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/swagger/public.swagger.json
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/tools/authfix.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/tools/func.txt
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/tools/old_func.txt
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/tools/swaggerfix.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/.gitignore
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/README.md
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 cudo_compute-0.1.7/PKG-INFO
+-rwxr-xr-x   0        0        0      706 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/codegen.sh
+-rw-r--r--   0        0        0   179499 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/fix.swagger.json
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/.github/workflows/workflow-test.yml
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0    27365 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/README.md
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/APIKeysApi.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ActivateBody.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/AddBillingAccountUserPermissionBody.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/AddDataCenterUserPermissionBody.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/AddProjectUserPermissionBody.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Any.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ApiKey.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/AttachSecurityGroupResponse.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/AttachStorageDiskResponse.md
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/BillingAccount.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/BillingAccountPaymentMethod.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/BillingAccountPaymentMethods.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/BillingAccountSetupIntent.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/BillingAccountSpendRow.md
+-rw-r--r--   0        0        0    19349 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/BillingApi.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Cluster.md
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ConnectVMResponse.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CountHostsResponse.md
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CountVMsResponse.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CpuModelCategory.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateBillingAccountRequest.md
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateDiskSnapshotBody.md
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateDiskSnapshotResponse.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateNetworkBody.md
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateNetworkResponse.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateObjectStorageUserBody.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreatePrivateVMImageResponse.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateSecurityGroupResponse.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateStorageDiskBody.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateStorageDiskResponse.md
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateVMBody.md
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateVMRequestNIC.md
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/CreateVMResponse.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DataCenter.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DataCenterCategory.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DataCenterRevenueResource.md
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DataCenterTimeRevenue.md
+-rw-r--r--   0        0        0    15819 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DataCentersApi.md
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Decimal.md
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DeleteDiskSnapshotResponse.md
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DeleteNetworkResponse.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DeleteObjectStorageKeyResponse.md
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DeleteObjectStorageUserResponse.md
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DeletePrivateVMImageResponse.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DeleteSecurityGroupResponse.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DeleteStorageDiskResponse.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DetachSecurityGroupResponse.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DetachStorageDiskResponse.md
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Disk.md
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DiskState.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DiskStorageClass.md
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DiskStoragePriceHr.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DiskType.md
+-rw-r--r--   0        0        0    14900 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/DisksApi.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GenerateApiKeyRequest.md
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetBillingAccountDetailsResponse.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetBillingAccountSpendDetailsResponse.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetBillingAccountStripeInvoicesResponse.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetDataCenterLiveUtilizationResponse.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetDataCenterRevenueByResourceResponse.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetDataCenterRevenueTimeSeriesResponse.md
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetDiskResponse.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetMachineTypeLiveUtilizationResponse.md
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetMachineTypeResponse.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetNetworkResponse.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetObjectStorageSessionKeyResponse.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetPrivateVMImageResponse.md
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetSecurityGroupResponse.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GetVMResponse.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/GpuModelCategory.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Host.md
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/HostConfigCategory.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/IdentityVerificationSession.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Image.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Interval.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Invoice.md
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListApiKeysResponse.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListBillingAccountsResponse.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListClustersResponse.md
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListDataCentersResponse.md
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListDiskSnapshotsResponse.md
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListDisksResponse.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListHostsResponse.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListMachineTypesResponse.md
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListNetworksResponse.md
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListObjectStorageBucketsResponse.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListObjectStorageKeysResponse.md
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListObjectStorageUsersResponse.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListOutstandingStripeInvoicesResponse.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListPrivateVMImagesResponse.md
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListPrivateVMImagesResponsePrivateImage.md
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListProjectSshKeysResponse.md
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListProjectsResponse.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListPublicVMImagesResponse.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListRegionsResponse.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListSecurityGroupsResponse.md
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListSshKeysResponse.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListUserPermissionsResponse.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListVMDataCentersResponse.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListVMDisksResponse.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListVMMachineTypesRequest.md
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListVMMachineTypesResponse.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ListVMsResponse.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/MachineType.md
+-rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/MachineTypesApi.md
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/MonitorVMResponse.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Network.md
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/NetworkPriceHr.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/NetworkState.md
+-rw-r--r--   0        0        0    16589 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/NetworksApi.md
+-rw-r--r--   0        0        0    16273 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ObjectStorageApi.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ObjectStorageBucket.md
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ObjectStorageKey.md
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ObjectStorageUser.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/PaymentMethodCard.md
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/PaymentMethodPaypal.md
+-rw-r--r--   0        0        0    12202 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/PermissionsApi.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Point.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Profile.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Project.md
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ProjectsApi.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Protocol.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/RebootVMResponse.md
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Region.md
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/RemoveBillingAccountPaymentMethodResponse.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/RemoveBillingAccountUserPermissionBody.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/RemoveDataCenterUserPermissionBody.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/RemoveProjectUserPermissionBody.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ResizeVMDiskResponse.md
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/ResizeVMResponse.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/RevertDiskResponse.md
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Role.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Rule.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/RuleType.md
+-rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/SSHKeysApi.md
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/SearchApi.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/SecurityGroup.md
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/SecurityGroup1.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/SecurityGroupRule.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/SetBillingAccountDefaultPaymentMethodResponse.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Snapshot.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/SshKey.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/SshKeySource.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/StartNetworkResponse.md
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/StartVMResponse.md
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Status.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/StopNetworkResponse.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/StopVMResponse.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/StripeCustomer.md
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/TaxId.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/TerminateVMResponse.md
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/Unit.md
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/UpdateBillingAccountBody.md
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/UpdatePrivateVMImageResponse.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/UpdateSecurityGroupResponse.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/UpdateVMMetadataBody.md
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/UpdateVMMetadataResponse.md
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/UserApi.md
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/UserPermission.md
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/V1PrivateImage.md
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/V1billingaccountsbillingAccountIdBillingAccount.md
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/VM.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/VMDataCenter.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/VMDataCenterStorageClass.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/VMMonitoringItem.md
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/VMNIC.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/VRouterSize.md
+-rw-r--r--   0        0        0    35782 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/VirtualMachinesApi.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/docs/VmState.md
+-rw-r--r--   0        0        0    13930 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/__init__.py
+-rw-r--r--   0        0        0    25117 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api_client.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/auth_config.py
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/configuration.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/cudo_api.py
+-rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/rest.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/__init__.py
+-rw-r--r--   0        0        0    12792 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/api_keys_api.py
+-rw-r--r--   0        0        0    55651 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/billing_api.py
+-rw-r--r--   0        0        0    48151 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/data_centers_api.py
+-rw-r--r--   0        0        0    48679 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/disks_api.py
+-rw-r--r--   0        0        0    14136 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/machine_types_api.py
+-rw-r--r--   0        0        0    52887 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/networks_api.py
+-rw-r--r--   0        0        0    47394 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/object_storage_api.py
+-rw-r--r--   0        0        0    35511 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/permissions_api.py
+-rw-r--r--   0        0        0    23477 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/projects_api.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/search_api.py
+-rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/ssh_keys_api.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/user_api.py
+-rw-r--r--   0        0        0   108047 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/api/virtual_machines_api.py
+-rw-r--r--   0        0        0    12902 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/__init__.py
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/activate_body.py
+-rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/add_billing_account_user_permission_body.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/add_data_center_user_permission_body.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/add_project_user_permission_body.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/any.py
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/api_key.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/attach_security_group_response.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/attach_storage_disk_response.py
+-rw-r--r--   0        0        0    10795 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/billing_account.py
+-rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/billing_account_payment_method.py
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/billing_account_payment_methods.py
+-rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/billing_account_setup_intent.py
+-rw-r--r--   0        0        0     7857 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/billing_account_spend_row.py
+-rw-r--r--   0        0        0    23208 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/cluster.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/connect_vm_response.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/count_hosts_response.py
+-rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/count_vms_response.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/cpu_model_category.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_billing_account_request.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_disk_snapshot_body.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_disk_snapshot_response.py
+-rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_network_body.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_network_response.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_object_storage_user_body.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_private_vm_image_response.py
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_security_group_response.py
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_storage_disk_body.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_storage_disk_response.py
+-rw-r--r--   0        0        0    16676 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_vm_body.py
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_vm_request_nic.py
+-rw-r--r--   0        0        0     3999 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/create_vm_response.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/data_center.py
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/data_center_category.py
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/data_center_revenue_resource.py
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/data_center_time_revenue.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/decimal.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_disk_snapshot_response.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_network_response.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_object_storage_key_response.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_object_storage_user_response.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_private_vm_image_response.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_security_group_response.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_storage_disk_response.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/detach_security_group_response.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/detach_storage_disk_response.py
+-rw-r--r--   0        0        0    10291 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/disk.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/disk_state.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/disk_storage_class.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/disk_storage_price_hr.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/disk_type.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/generate_api_key_request.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_billing_account_details_response.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_billing_account_spend_details_response.py
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_billing_account_stripe_invoices_response.py
+-rw-r--r--   0        0        0    15542 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_data_center_live_utilization_response.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_data_center_revenue_by_resource_response.py
+-rw-r--r--   0        0        0     3928 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_data_center_revenue_time_series_response.py
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_disk_response.py
+-rw-r--r--   0        0        0    15599 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_machine_type_live_utilization_response.py
+-rw-r--r--   0        0        0    21098 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_machine_type_response.py
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_network_response.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_object_storage_session_key_response.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_private_vm_image_response.py
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_security_group_response.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/get_vm_response.py
+-rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/gpu_model_category.py
+-rw-r--r--   0        0        0    14802 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/host.py
+-rw-r--r--   0        0        0    19137 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/host_config_category.py
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/identity_verification_session.py
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/image.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/interval.py
+-rw-r--r--   0        0        0    13547 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/invoice.py
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_billing_accounts_response.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_clusters_response.py
+-rw-r--r--   0        0        0     5491 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_data_centers_response.py
+-rw-r--r--   0        0        0     3710 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_disk_snapshots_response.py
+-rw-r--r--   0        0        0     5988 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_disks_response.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_hosts_response.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_machine_types_response.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_networks_response.py
+-rw-r--r--   0        0        0     6521 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_object_storage_buckets_response.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_object_storage_keys_response.py
+-rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_object_storage_users_response.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_outstanding_stripe_invoices_response.py
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_private_vm_images_response.py
+-rw-r--r--   0        0        0     6804 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_private_vm_images_response_private_image.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_project_ssh_keys_response.py
+-rw-r--r--   0        0        0     5348 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_projects_response.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_public_vm_images_response.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_regions_response.py
+-rw-r--r--   0        0        0     6544 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_security_groups_response.py
+-rw-r--r--   0        0        0     6229 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_ssh_keys_response.py
+-rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_user_permissions_response.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_vm_data_centers_response.py
+-rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_vm_disks_response.py
+-rw-r--r--   0        0        0    11819 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_vm_machine_types_request.py
+-rw-r--r--   0        0        0    11283 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_vm_machine_types_response.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/list_vms_response.py
+-rw-r--r--   0        0        0     7406 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/machine_type.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/monitor_vm_response.py
+-rw-r--r--   0        0        0    11038 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/network.py
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/network_price_hr.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/network_state.py
+-rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/object_storage_bucket.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/object_storage_key.py
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/object_storage_user.py
+-rw-r--r--   0        0        0     6773 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/payment_method_card.py
+-rw-r--r--   0        0        0     4211 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/payment_method_paypal.py
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/point.py
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/profile.py
+-rw-r--r--   0        0        0     5114 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/project.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/protocol.py
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/reboot_vm_response.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/region.py
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/remove_billing_account_payment_method_response.py
+-rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/remove_billing_account_user_permission_body.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/remove_data_center_user_permission_body.py
+-rw-r--r--   0        0        0     6256 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/remove_project_user_permission_body.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/resize_vm_disk_response.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/resize_vm_response.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/revert_disk_response.py
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/role.py
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/rule.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/rule_type.py
+-rw-r--r--   0        0        0     5684 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/security_group.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/security_group1.py
+-rw-r--r--   0        0        0     6821 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/security_group_rule.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/set_billing_account_default_payment_method_response.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/snapshot.py
+-rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/ssh_key.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/ssh_key_source.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/start_network_response.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/start_vm_response.py
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/status.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/stop_network_response.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/stop_vm_response.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/stripe_customer.py
+-rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/tax_id.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/terminate_vm_response.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/unit.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/update_billing_account_body.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/update_private_vm_image_response.py
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/update_security_group_response.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/update_vm_metadata_body.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/update_vm_metadata_response.py
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/user_permission.py
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/v1_private_image.py
+-rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/v_router_size.py
+-rw-r--r--   0        0        0    25899 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/vm.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/vm_data_center.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/vm_data_center_storage_class.py
+-rw-r--r--   0        0        0     8981 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/vm_monitoring_item.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/vm_state.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/docs/src/cudo_compute/models/vmnic.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/examples/create-vm.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/examples/get-vm.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/examples/images.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/examples/list-vms.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/examples/machine-types.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/examples/terminate-vm.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/helpers/auth_config.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/helpers/cudo_api.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/.gitignore
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/.swagger-codegen-ignore
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/.travis.yml
+-rw-r--r--   0        0        0    27337 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/README.md
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/git_push.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/requirements.txt
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/setup.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test-requirements.txt
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/tox.ini
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/__init__.py
+-rw-r--r--   0        0        0    25101 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api_client.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/configuration.py
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/rest.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/__init__.py
+-rw-r--r--   0        0        0    12788 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/api_keys_api.py
+-rw-r--r--   0        0        0    55647 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/billing_api.py
+-rw-r--r--   0        0        0    48147 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/data_centers_api.py
+-rw-r--r--   0        0        0    48675 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/disks_api.py
+-rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/machine_types_api.py
+-rw-r--r--   0        0        0    52883 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/networks_api.py
+-rw-r--r--   0        0        0    47390 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/object_storage_api.py
+-rw-r--r--   0        0        0    35507 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/permissions_api.py
+-rw-r--r--   0        0        0    23473 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/projects_api.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/search_api.py
+-rw-r--r--   0        0        0    15226 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/ssh_keys_api.py
+-rw-r--r--   0        0        0    10783 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/user_api.py
+-rw-r--r--   0        0        0   108043 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/api/virtual_machines_api.py
+-rw-r--r--   0        0        0    12278 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/activate_body.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/add_billing_account_user_permission_body.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/add_data_center_user_permission_body.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/add_project_user_permission_body.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/any.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/api_key.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/attach_security_group_response.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/attach_storage_disk_response.py
+-rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/billing_account.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/billing_account_payment_method.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/billing_account_payment_methods.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/billing_account_setup_intent.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/billing_account_spend_row.py
+-rw-r--r--   0        0        0    23204 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/cluster.py
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/connect_vm_response.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/count_hosts_response.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/count_vms_response.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/cpu_model_category.py
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_billing_account_request.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_disk_snapshot_body.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_disk_snapshot_response.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_network_body.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_network_response.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_object_storage_user_body.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_private_vm_image_response.py
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_security_group_response.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_storage_disk_body.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_storage_disk_response.py
+-rw-r--r--   0        0        0    16672 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_vm_body.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_vm_request_nic.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/create_vm_response.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/data_center.py
+-rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/data_center_category.py
+-rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/data_center_revenue_resource.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/data_center_time_revenue.py
+-rw-r--r--   0        0        0     8588 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/decimal.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/delete_disk_snapshot_response.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/delete_network_response.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/delete_object_storage_key_response.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/delete_object_storage_user_response.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/delete_private_vm_image_response.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/delete_security_group_response.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/delete_storage_disk_response.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/detach_security_group_response.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/detach_storage_disk_response.py
+-rw-r--r--   0        0        0    10287 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/disk.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/disk_state.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/disk_storage_class.py
+-rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/disk_storage_price_hr.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/disk_type.py
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/generate_api_key_request.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_billing_account_details_response.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_billing_account_spend_details_response.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_billing_account_stripe_invoices_response.py
+-rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_data_center_live_utilization_response.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_data_center_revenue_by_resource_response.py
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_data_center_revenue_time_series_response.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_disk_response.py
+-rw-r--r--   0        0        0    15595 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_machine_type_live_utilization_response.py
+-rw-r--r--   0        0        0    21094 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_machine_type_response.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_network_response.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_object_storage_session_key_response.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_private_vm_image_response.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_security_group_response.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/get_vm_response.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/gpu_model_category.py
+-rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/host.py
+-rw-r--r--   0        0        0    19133 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/host_config_category.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/identity_verification_session.py
+-rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/image.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/interval.py
+-rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/invoice.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_billing_accounts_response.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_clusters_response.py
+-rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_data_centers_response.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_disk_snapshots_response.py
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_disks_response.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_hosts_response.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_machine_types_response.py
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_networks_response.py
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_object_storage_buckets_response.py
+-rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_object_storage_keys_response.py
+-rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_object_storage_users_response.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_outstanding_stripe_invoices_response.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_private_vm_images_response.py
+-rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_private_vm_images_response_private_image.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_project_ssh_keys_response.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_projects_response.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_public_vm_images_response.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_regions_response.py
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_security_groups_response.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_ssh_keys_response.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_user_permissions_response.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_vm_data_centers_response.py
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_vm_disks_response.py
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_vm_machine_types_request.py
+-rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_vm_machine_types_response.py
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/list_vms_response.py
+-rw-r--r--   0        0        0     7402 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/machine_type.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/monitor_vm_response.py
+-rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/network.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/network_price_hr.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/network_state.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/object_storage_bucket.py
+-rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/object_storage_key.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/object_storage_user.py
+-rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/payment_method_card.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/payment_method_paypal.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/point.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/profile.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/project.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/protocol.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/reboot_vm_response.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/region.py
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/remove_billing_account_payment_method_response.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/remove_billing_account_user_permission_body.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/remove_data_center_user_permission_body.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/remove_project_user_permission_body.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/resize_vm_disk_response.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/resize_vm_response.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/revert_disk_response.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/role.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/rule.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/rule_type.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/security_group.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/security_group1.py
+-rw-r--r--   0        0        0     6817 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/security_group_rule.py
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/set_billing_account_default_payment_method_response.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/snapshot.py
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/ssh_key.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/ssh_key_source.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/start_network_response.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/start_vm_response.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/status.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/stop_network_response.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/stop_vm_response.py
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/stripe_customer.py
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/tax_id.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/terminate_vm_response.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/unit.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/update_billing_account_body.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/update_private_vm_image_response.py
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/update_security_group_response.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/update_vm_metadata_body.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/update_vm_metadata_response.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/user_permission.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/v1_private_image.py
+-rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/v_router_size.py
+-rw-r--r--   0        0        0    25895 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/vm.py
+-rw-r--r--   0        0        0     8588 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/vm_data_center.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/vm_data_center_storage_class.py
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/vm_monitoring_item.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/vm_state.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/cudo_compute/models/vmnic.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/APIKeysApi.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ActivateBody.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/AddBillingAccountUserPermissionBody.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/AddDataCenterUserPermissionBody.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/AddProjectUserPermissionBody.md
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Any.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ApiKey.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/AttachSecurityGroupResponse.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/AttachStorageDiskResponse.md
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/BillingAccount.md
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/BillingAccountPaymentMethod.md
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/BillingAccountPaymentMethods.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/BillingAccountSetupIntent.md
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/BillingAccountSpendRow.md
+-rw-r--r--   0        0        0    19181 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/BillingApi.md
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Cluster.md
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ConnectVMResponse.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CountHostsResponse.md
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CountVMsResponse.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CpuModelCategory.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateBillingAccountRequest.md
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateDiskSnapshotBody.md
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateDiskSnapshotResponse.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateNetworkBody.md
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateNetworkResponse.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateObjectStorageUserBody.md
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreatePrivateVMImageResponse.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateSecurityGroupResponse.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateStorageDiskBody.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateStorageDiskResponse.md
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateVMBody.md
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateVMRequestNIC.md
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/CreateVMResponse.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DataCenter.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DataCenterCategory.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DataCenterRevenueResource.md
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DataCenterTimeRevenue.md
+-rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DataCentersApi.md
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Decimal.md
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DeleteDiskSnapshotResponse.md
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DeleteNetworkResponse.md
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DeleteObjectStorageKeyResponse.md
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DeleteObjectStorageUserResponse.md
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DeletePrivateVMImageResponse.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DeleteSecurityGroupResponse.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DeleteStorageDiskResponse.md
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DetachSecurityGroupResponse.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DetachStorageDiskResponse.md
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Disk.md
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DiskState.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DiskStorageClass.md
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DiskStoragePriceHr.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DiskType.md
+-rw-r--r--   0        0        0    14768 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/DisksApi.md
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GenerateApiKeyRequest.md
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetBillingAccountDetailsResponse.md
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetBillingAccountSpendDetailsResponse.md
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetBillingAccountStripeInvoicesResponse.md
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetDataCenterLiveUtilizationResponse.md
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetDataCenterRevenueByResourceResponse.md
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetDataCenterRevenueTimeSeriesResponse.md
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetDiskResponse.md
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetMachineTypeLiveUtilizationResponse.md
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetMachineTypeResponse.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetNetworkResponse.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetObjectStorageSessionKeyResponse.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetPrivateVMImageResponse.md
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetSecurityGroupResponse.md
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GetVMResponse.md
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/GpuModelCategory.md
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Host.md
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/HostConfigCategory.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/IdentityVerificationSession.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Image.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Interval.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Invoice.md
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListApiKeysResponse.md
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListBillingAccountsResponse.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListClustersResponse.md
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListDataCentersResponse.md
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListDiskSnapshotsResponse.md
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListDisksResponse.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListHostsResponse.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListMachineTypesResponse.md
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListNetworksResponse.md
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListObjectStorageBucketsResponse.md
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListObjectStorageKeysResponse.md
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListObjectStorageUsersResponse.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListOutstandingStripeInvoicesResponse.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListPrivateVMImagesResponse.md
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListPrivateVMImagesResponsePrivateImage.md
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListProjectSshKeysResponse.md
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListProjectsResponse.md
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListPublicVMImagesResponse.md
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListRegionsResponse.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListSecurityGroupsResponse.md
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListSshKeysResponse.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListUserPermissionsResponse.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListVMDataCentersResponse.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListVMDisksResponse.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListVMMachineTypesRequest.md
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListVMMachineTypesResponse.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ListVMsResponse.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/MachineType.md
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/MachineTypesApi.md
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/MonitorVMResponse.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Network.md
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/NetworkPriceHr.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/NetworkState.md
+-rw-r--r--   0        0        0    16441 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/NetworksApi.md
+-rw-r--r--   0        0        0    16141 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ObjectStorageApi.md
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ObjectStorageBucket.md
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ObjectStorageKey.md
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ObjectStorageUser.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/PaymentMethodCard.md
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/PaymentMethodPaypal.md
+-rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/PermissionsApi.md
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Point.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Profile.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Project.md
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ProjectsApi.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Protocol.md
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/RebootVMResponse.md
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Region.md
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/RemoveBillingAccountPaymentMethodResponse.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/RemoveBillingAccountUserPermissionBody.md
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/RemoveDataCenterUserPermissionBody.md
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/RemoveProjectUserPermissionBody.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ResizeVMDiskResponse.md
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/ResizeVMResponse.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/RevertDiskResponse.md
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Role.md
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Rule.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/RuleType.md
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/SSHKeysApi.md
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/SearchApi.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/SecurityGroup.md
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/SecurityGroup1.md
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/SecurityGroupRule.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/SetBillingAccountDefaultPaymentMethodResponse.md
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Snapshot.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/SshKey.md
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/SshKeySource.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/StartNetworkResponse.md
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/StartVMResponse.md
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Status.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/StopNetworkResponse.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/StopVMResponse.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/StripeCustomer.md
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/TaxId.md
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/TerminateVMResponse.md
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/Unit.md
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/UpdateBillingAccountBody.md
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/UpdatePrivateVMImageResponse.md
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/UpdateSecurityGroupResponse.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/UpdateVMMetadataBody.md
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/UpdateVMMetadataResponse.md
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/UserApi.md
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/UserPermission.md
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/V1PrivateImage.md
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/V1billingaccountsbillingAccountIdBillingAccount.md
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/VM.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/VMDataCenter.md
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/VMDataCenterStorageClass.md
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/VMMonitoringItem.md
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/VMNIC.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/VRouterSize.md
+-rw-r--r--   0        0        0    35482 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/VirtualMachinesApi.md
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/docs/VmState.md
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/__init__.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_activate_body.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_add_billing_account_user_permission_body.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_add_data_center_user_permission_body.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_add_project_user_permission_body.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_any.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_api_key.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_api_keys_api.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_attach_security_group_response.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_attach_storage_disk_response.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_billing_account.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_billing_account_payment_method.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_billing_account_payment_methods.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_billing_account_setup_intent.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_billing_account_spend_row.py
+-rw-r--r--   0        0        0     3021 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_billing_api.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_cluster.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_connect_vm_response.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_count_hosts_response.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_count_vms_response.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_cpu_model_category.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_billing_account_request.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_disk_snapshot_body.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_disk_snapshot_response.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_network_body.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_network_response.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_object_storage_user_body.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_private_vm_image_response.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_security_group_response.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_storage_disk_body.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_storage_disk_response.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_vm_body.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_vm_request_nic.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_create_vm_response.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_data_center.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_data_center_category.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_data_center_revenue_resource.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_data_center_time_revenue.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_data_centers_api.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_decimal.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_delete_disk_snapshot_response.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_delete_network_response.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_delete_object_storage_key_response.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_delete_object_storage_user_response.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_delete_private_vm_image_response.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_delete_security_group_response.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_delete_storage_disk_response.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_detach_security_group_response.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_detach_storage_disk_response.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_disk.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_disk_state.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_disk_storage_class.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_disk_storage_price_hr.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_disk_type.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_disks_api.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_generate_api_key_request.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_billing_account_details_response.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_billing_account_spend_details_response.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_billing_account_stripe_invoices_response.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_data_center_live_utilization_response.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_data_center_revenue_by_resource_response.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_data_center_revenue_time_series_response.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_disk_response.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_machine_type_live_utilization_response.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_machine_type_response.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_network_response.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_object_storage_session_key_response.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_private_vm_image_response.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_security_group_response.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_get_vm_response.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_gpu_model_category.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_host.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_host_config_category.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_identity_verification_session.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_image.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_interval.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_invoice.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_api_keys_response.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_billing_accounts_response.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_clusters_response.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_data_centers_response.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_disk_snapshots_response.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_disks_response.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_hosts_response.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_machine_types_response.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_networks_response.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_object_storage_buckets_response.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_object_storage_keys_response.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_object_storage_users_response.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_outstanding_stripe_invoices_response.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_private_vm_images_response.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_private_vm_images_response_private_image.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_project_ssh_keys_response.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_projects_response.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_public_vm_images_response.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_regions_response.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_security_groups_response.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_ssh_keys_response.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_user_permissions_response.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_vm_data_centers_response.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_vm_disks_response.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_vm_machine_types_request.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_vm_machine_types_response.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_list_vms_response.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_machine_type.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_machine_types_api.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_monitor_vm_response.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_network.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_network_price_hr.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_network_state.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_networks_api.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_object_storage_api.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_object_storage_bucket.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_object_storage_key.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_object_storage_user.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_payment_method_card.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_payment_method_paypal.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_permissions_api.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_point.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_profile.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_project.py
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_projects_api.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_protocol.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_reboot_vm_response.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_region.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_remove_billing_account_payment_method_response.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_remove_billing_account_user_permission_body.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_remove_data_center_user_permission_body.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_remove_project_user_permission_body.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_resize_vm_disk_response.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_resize_vm_response.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_revert_disk_response.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_role.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_rule.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_rule_type.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_search_api.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_security_group.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_security_group1.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_security_group_rule.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_set_billing_account_default_payment_method_response.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_snapshot.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_ssh_key.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_ssh_key_source.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_ssh_keys_api.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_start_network_response.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_start_vm_response.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_status.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_stop_network_response.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_stop_vm_response.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_stripe_customer.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_tax_id.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_terminate_vm_response.py
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_unit.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_update_billing_account_body.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_update_private_vm_image_response.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_update_security_group_response.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_update_vm_metadata_body.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_update_vm_metadata_response.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_user_api.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_user_permission.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_v1_private_image.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_v1billingaccountsbilling_account_id_billing_account.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_v_router_size.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_virtual_machines_api.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_vm.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_vm_data_center.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_vm_data_center_storage_class.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_vm_monitoring_item.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_vm_state.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/out/test/test_vmnic.py
+-rw-r--r--   0        0        0    13242 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/__init__.py
+-rw-r--r--   0        0        0    25101 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api_client.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/auth_config.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/configuration.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/cudo_api.py
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/rest.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/__init__.py
+-rw-r--r--   0        0        0    12791 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/api_keys_api.py
+-rw-r--r--   0        0        0    55660 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/billing_api.py
+-rw-r--r--   0        0        0    48158 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/data_centers_api.py
+-rw-r--r--   0        0        0    48685 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/disks_api.py
+-rw-r--r--   0        0        0    14135 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/machine_types_api.py
+-rw-r--r--   0        0        0    52894 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/networks_api.py
+-rw-r--r--   0        0        0    47400 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/object_storage_api.py
+-rw-r--r--   0        0        0    35514 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/permissions_api.py
+-rw-r--r--   0        0        0    23479 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/projects_api.py
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/search_api.py
+-rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/ssh_keys_api.py
+-rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/user_api.py
+-rw-r--r--   0        0        0   108067 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/api/virtual_machines_api.py
+-rw-r--r--   0        0        0    12278 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/__init__.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/activate_body.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/add_billing_account_user_permission_body.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/add_data_center_user_permission_body.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/add_project_user_permission_body.py
+-rw-r--r--   0        0        0     3241 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/any.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/api_key.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/attach_security_group_response.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/attach_storage_disk_response.py
+-rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/billing_account.py
+-rw-r--r--   0        0        0     6216 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/billing_account_payment_method.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/billing_account_payment_methods.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/billing_account_setup_intent.py
+-rw-r--r--   0        0        0     7853 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/billing_account_spend_row.py
+-rw-r--r--   0        0        0    23204 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/cluster.py
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/connect_vm_response.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/count_hosts_response.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/count_vms_response.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/cpu_model_category.py
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_billing_account_request.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_disk_snapshot_body.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_disk_snapshot_response.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_network_body.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_network_response.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_object_storage_user_body.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_private_vm_image_response.py
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_security_group_response.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_storage_disk_body.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_storage_disk_response.py
+-rw-r--r--   0        0        0    16672 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_vm_body.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_vm_request_nic.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/create_vm_response.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/data_center.py
+-rw-r--r--   0        0        0     6380 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/data_center_category.py
+-rw-r--r--   0        0        0     7192 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/data_center_revenue_resource.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/data_center_time_revenue.py
+-rw-r--r--   0        0        0     8588 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/decimal.py
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/delete_disk_snapshot_response.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/delete_network_response.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/delete_object_storage_key_response.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/delete_object_storage_user_response.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/delete_private_vm_image_response.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/delete_security_group_response.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/delete_storage_disk_response.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/detach_security_group_response.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/detach_storage_disk_response.py
+-rw-r--r--   0        0        0    10287 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/disk.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/disk_state.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/disk_storage_class.py
+-rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/disk_storage_price_hr.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/disk_type.py
+-rw-r--r--   0        0        0     4054 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/generate_api_key_request.py
+-rw-r--r--   0        0        0     4944 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_billing_account_details_response.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_billing_account_spend_details_response.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_billing_account_stripe_invoices_response.py
+-rw-r--r--   0        0        0    15538 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_data_center_live_utilization_response.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_data_center_revenue_by_resource_response.py
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_data_center_revenue_time_series_response.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_disk_response.py
+-rw-r--r--   0        0        0    15595 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_machine_type_live_utilization_response.py
+-rw-r--r--   0        0        0    21094 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_machine_type_response.py
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_network_response.py
+-rw-r--r--   0        0        0     6835 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_object_storage_session_key_response.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_private_vm_image_response.py
+-rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_security_group_response.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/get_vm_response.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/gpu_model_category.py
+-rw-r--r--   0        0        0    14798 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/host.py
+-rw-r--r--   0        0        0    19133 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/host_config_category.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/identity_verification_session.py
+-rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/image.py
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/interval.py
+-rw-r--r--   0        0        0    13543 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/invoice.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_billing_accounts_response.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_clusters_response.py
+-rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_data_centers_response.py
+-rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_disk_snapshots_response.py
+-rw-r--r--   0        0        0     5984 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_disks_response.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_hosts_response.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_machine_types_response.py
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_networks_response.py
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_object_storage_buckets_response.py
+-rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_object_storage_keys_response.py
+-rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_object_storage_users_response.py
+-rw-r--r--   0        0        0     3790 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_outstanding_stripe_invoices_response.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_private_vm_images_response.py
+-rw-r--r--   0        0        0     6800 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_private_vm_images_response_private_image.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_project_ssh_keys_response.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_projects_response.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_public_vm_images_response.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_regions_response.py
+-rw-r--r--   0        0        0     6540 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_security_groups_response.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_ssh_keys_response.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_user_permissions_response.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_vm_data_centers_response.py
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_vm_disks_response.py
+-rw-r--r--   0        0        0    11815 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_vm_machine_types_request.py
+-rw-r--r--   0        0        0    11279 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_vm_machine_types_response.py
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/list_vms_response.py
+-rw-r--r--   0        0        0     7402 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/machine_type.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/monitor_vm_response.py
+-rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/network.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/network_price_hr.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/network_state.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/object_storage_bucket.py
+-rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/object_storage_key.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/object_storage_user.py
+-rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/payment_method_card.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/payment_method_paypal.py
+-rw-r--r--   0        0        0     3779 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/point.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/profile.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/project.py
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/protocol.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/reboot_vm_response.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/region.py
+-rw-r--r--   0        0        0     4764 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/remove_billing_account_payment_method_response.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/remove_billing_account_user_permission_body.py
+-rw-r--r--   0        0        0     6236 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/remove_data_center_user_permission_body.py
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/remove_project_user_permission_body.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/resize_vm_disk_response.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/resize_vm_response.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/revert_disk_response.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/role.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/rule.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/rule_type.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/security_group.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/security_group1.py
+-rw-r--r--   0        0        0     6817 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/security_group_rule.py
+-rw-r--r--   0        0        0     4816 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/set_billing_account_default_payment_method_response.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/snapshot.py
+-rw-r--r--   0        0        0     6601 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/ssh_key.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/ssh_key_source.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/start_network_response.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/start_vm_response.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/status.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/stop_network_response.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/stop_vm_response.py
+-rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/stripe_customer.py
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/tax_id.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/terminate_vm_response.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/unit.py
+-rw-r--r--   0        0        0     4681 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/update_billing_account_body.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/update_private_vm_image_response.py
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/update_security_group_response.py
+-rw-r--r--   0        0        0     4138 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/update_vm_metadata_body.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/update_vm_metadata_response.py
+-rw-r--r--   0        0        0     6916 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/user_permission.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/v1_private_image.py
+-rw-r--r--   0        0        0    11731 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/v_router_size.py
+-rw-r--r--   0        0        0    25895 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/vm.py
+-rw-r--r--   0        0        0     8588 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/vm_data_center.py
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/vm_data_center_storage_class.py
+-rw-r--r--   0        0        0     8977 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/vm_monitoring_item.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/vm_state.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/src/cudo_compute/models/vmnic.py
+-rw-r--r--   0        0        0   179189 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/swagger/public.swagger.json
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/tools/authfix.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/tools/func.txt
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/tools/old_func.txt
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/tools/swaggerfix.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/.gitignore
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/README.md
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 cudo_compute-0.1.8/PKG-INFO
```

### Comparing `cudo_compute-0.1.7/codegen.sh` & `cudo_compute-0.1.8/codegen.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 python3 tools/swaggerfix.py
 
 rm -rf src
+mkdir src
 rm -rf swagger-codegen
 git clone https://github.com/swagger-api/swagger-codegen
 mv fix.swagger.json swagger-codegen
 
 cd swagger-codegen
 ./run-in-docker.sh mvn package
 ./run-in-docker.sh generate -i fix.swagger.json \
@@ -12,11 +13,11 @@
 cd ..
 cp swagger-codegen/out/README.md docs
 cp -r swagger-codegen/out/docs/ docs
 cp -r swagger-codegen/out/src/ docs
 #rm -rf swagger-codegen
 
 cp helpers/* docs/src/cudo_compute
-echo "import src.cudo_compute.auth_config as AuthConfig" >> src/cudo_compute/__init__.py
-echo "import cudo_compute.cudo_api as cudo_api" >> src/cudo_compute/__init__.py
+echo "import src.cudo_compute.auth_config as AuthConfig" >> docs/src/cudo_compute/__init__.py
+echo "import cudo_compute.cudo_api as cudo_api" >> docs/src/cudo_compute/__init__.py
 
-python3 tools/authfix.py
+#python3 tools/authfix.py
```

### Comparing `cudo_compute-0.1.7/fix.swagger.json` & `cudo_compute-0.1.8/fix.swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999813988095239%*

 * *Differences: {"'definitions'": "{'Disk': {'required': {delete: [0]}}}"}*

```diff
@@ -609,15 +609,14 @@
                 },
                 "vmId": {
                     "readOnly": true,
                     "type": "string"
                 }
             },
             "required": [
-                "id",
                 "sizeGib"
             ],
             "type": "object"
         },
         "Disk.StorageClass": {
             "default": "STORAGE_CLASS_UNKNOWN",
             "enum": [
```

### Comparing `cudo_compute-0.1.7/.github/workflows/workflow-test.yml` & `cudo_compute-0.1.8/.github/workflows/workflow-test.yml`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/.github/workflows/workflow.yml` & `cudo_compute-0.1.8/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/README.md` & `cudo_compute-0.1.8/docs/README.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/APIKeysApi.md` & `cudo_compute-0.1.8/docs/docs/APIKeysApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/BillingAccount.md` & `cudo_compute-0.1.8/docs/docs/BillingAccount.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/BillingAccountPaymentMethod.md` & `cudo_compute-0.1.8/docs/docs/BillingAccountPaymentMethod.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/BillingAccountSpendRow.md` & `cudo_compute-0.1.8/docs/docs/BillingAccountSpendRow.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/BillingApi.md` & `cudo_compute-0.1.8/docs/docs/BillingApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/Cluster.md` & `cudo_compute-0.1.8/docs/docs/Cluster.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/CreateVMBody.md` & `cudo_compute-0.1.8/docs/docs/CreateVMBody.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/DataCenter.md` & `cudo_compute-0.1.8/docs/docs/DataCenter.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/DataCentersApi.md` & `cudo_compute-0.1.8/docs/docs/DataCentersApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/Decimal.md` & `cudo_compute-0.1.8/docs/docs/Decimal.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/Disk.md` & `cudo_compute-0.1.8/docs/docs/Disk.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **create_time** | **datetime** |  | [optional] 
 **data_center_id** | **str** |  | [optional] 
 **disk_state** | [**DiskState**](DiskState.md) |  | [optional] 
 **disk_type** | [**DiskType**](DiskType.md) |  | [optional] 
-**id** | **str** |  | 
+**id** | **str** |  | [optional] 
 **private_image_id** | **str** |  | [optional] 
 **project_id** | **str** |  | [optional] 
 **public_image_id** | **str** |  | [optional] 
 **size_gib** | **int** |  | 
 **storage_class** | [**DiskStorageClass**](DiskStorageClass.md) |  | [optional] 
 **vm_id** | **str** |  | [optional]
```

### Comparing `cudo_compute-0.1.7/docs/docs/DiskStoragePriceHr.md` & `cudo_compute-0.1.8/docs/docs/DiskStoragePriceHr.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/DisksApi.md` & `cudo_compute-0.1.8/docs/docs/DisksApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/GenerateApiKeyRequest.md` & `cudo_compute-0.1.8/docs/docs/GenerateApiKeyRequest.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/GetDataCenterLiveUtilizationResponse.md` & `cudo_compute-0.1.8/docs/docs/GetDataCenterLiveUtilizationResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/GetMachineTypeLiveUtilizationResponse.md` & `cudo_compute-0.1.8/docs/docs/GetMachineTypeLiveUtilizationResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/GetMachineTypeResponse.md` & `cudo_compute-0.1.8/docs/docs/GetMachineTypeResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/GetObjectStorageSessionKeyResponse.md` & `cudo_compute-0.1.8/docs/docs/GetObjectStorageSessionKeyResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/Host.md` & `cudo_compute-0.1.8/docs/docs/Host.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/HostConfigCategory.md` & `cudo_compute-0.1.8/docs/docs/HostConfigCategory.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/Invoice.md` & `cudo_compute-0.1.8/docs/docs/Invoice.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/ListPrivateVMImagesResponse.md` & `cudo_compute-0.1.8/docs/docs/ListPrivateVMImagesResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/ListPrivateVMImagesResponsePrivateImage.md` & `cudo_compute-0.1.8/docs/docs/ListPrivateVMImagesResponsePrivateImage.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/ListUserPermissionsResponse.md` & `cudo_compute-0.1.8/docs/docs/ListUserPermissionsResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/ListVMMachineTypesRequest.md` & `cudo_compute-0.1.8/docs/docs/ListVMMachineTypesRequest.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/ListVMMachineTypesResponse.md` & `cudo_compute-0.1.8/docs/docs/ListVMMachineTypesResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/MachineTypesApi.md` & `cudo_compute-0.1.8/docs/docs/MachineTypesApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/Network.md` & `cudo_compute-0.1.8/docs/docs/Network.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/NetworksApi.md` & `cudo_compute-0.1.8/docs/docs/NetworksApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/ObjectStorageApi.md` & `cudo_compute-0.1.8/docs/docs/ObjectStorageApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/ObjectStorageBucket.md` & `cudo_compute-0.1.8/docs/docs/ObjectStorageBucket.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/PaymentMethodCard.md` & `cudo_compute-0.1.8/docs/docs/PaymentMethodCard.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/PermissionsApi.md` & `cudo_compute-0.1.8/docs/docs/PermissionsApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/ProjectsApi.md` & `cudo_compute-0.1.8/docs/docs/ProjectsApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/Rule.md` & `cudo_compute-0.1.8/docs/docs/Rule.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/SSHKeysApi.md` & `cudo_compute-0.1.8/docs/docs/SSHKeysApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/SearchApi.md` & `cudo_compute-0.1.8/docs/docs/SearchApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/SecurityGroupRule.md` & `cudo_compute-0.1.8/docs/docs/SecurityGroupRule.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/SshKey.md` & `cudo_compute-0.1.8/docs/docs/SshKey.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/UserApi.md` & `cudo_compute-0.1.8/docs/docs/UserApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/V1billingaccountsbillingAccountIdBillingAccount.md` & `cudo_compute-0.1.8/docs/docs/V1billingaccountsbillingAccountIdBillingAccount.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/VM.md` & `cudo_compute-0.1.8/docs/docs/VM.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/VMDataCenter.md` & `cudo_compute-0.1.8/docs/docs/VMDataCenter.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/VMMonitoringItem.md` & `cudo_compute-0.1.8/docs/docs/VMMonitoringItem.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/VMNIC.md` & `cudo_compute-0.1.8/docs/docs/VMNIC.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/docs/VirtualMachinesApi.md` & `cudo_compute-0.1.8/docs/docs/VirtualMachinesApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/__init__.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 # import apis into sdk package
 from src.cudo_compute.api.api_keys_api import APIKeysApi
 from src.cudo_compute.api.billing_api import BillingApi
 from src.cudo_compute.api.data_centers_api import DataCentersApi
 from src.cudo_compute.api.disks_api import DisksApi
@@ -185,7 +186,9 @@
 from src.cudo_compute.models.vm import VM
 from src.cudo_compute.models.vm_data_center import VMDataCenter
 from src.cudo_compute.models.vm_data_center_storage_class import VMDataCenterStorageClass
 from src.cudo_compute.models.vm_monitoring_item import VMMonitoringItem
 from src.cudo_compute.models.vmnic import VMNIC
 from src.cudo_compute.models.v_router_size import VRouterSize
 from src.cudo_compute.models.vm_state import VmState
+import src.cudo_compute.auth_config as AuthConfig
+import cudo_compute.cudo_api as cudo_api
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api_client.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
+
 from __future__ import absolute_import
 
 import datetime
 import json
 import mimetypes
 from multiprocessing.pool import ThreadPool
 import os
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/auth_config.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/auth_config.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/configuration.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/cudo_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/cudo_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/rest.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import io
 import json
 import logging
 import re
 import ssl
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/__init__.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/api_keys_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/api_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/billing_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/billing_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/data_centers_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/data_centers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/disks_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/disks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/machine_types_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/machine_types_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/networks_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/networks_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/object_storage_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/object_storage_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/permissions_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/permissions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/projects_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/projects_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/search_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/search_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/ssh_keys_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/ssh_keys_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/user_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/api/virtual_machines_api.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/api/virtual_machines_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 # python 2 and python 3 compatibility library
 import six
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/__init__.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 from __future__ import absolute_import
 
 # import models into model package
 from src.cudo_compute.models.activate_body import ActivateBody
 from src.cudo_compute.models.add_billing_account_user_permission_body import AddBillingAccountUserPermissionBody
 from src.cudo_compute.models.add_data_center_user_permission_body import AddDataCenterUserPermissionBody
 from src.cudo_compute.models.add_project_user_permission_body import AddProjectUserPermissionBody
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/activate_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/activate_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/add_billing_account_user_permission_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/add_billing_account_user_permission_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/add_data_center_user_permission_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/add_data_center_user_permission_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/add_project_user_permission_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/add_project_user_permission_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/any.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/any.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/api_key.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/attach_security_group_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/attach_security_group_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/attach_storage_disk_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/attach_storage_disk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/billing_account.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/billing_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/billing_account_payment_method.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/billing_account_payment_method.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/billing_account_payment_methods.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/billing_account_payment_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/billing_account_setup_intent.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/billing_account_setup_intent.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/billing_account_spend_row.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/billing_account_spend_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/cluster.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/cluster.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/connect_vm_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/connect_vm_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/count_hosts_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/count_hosts_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/count_vms_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/count_vms_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/cpu_model_category.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/cpu_model_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_billing_account_request.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_billing_account_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_disk_snapshot_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_disk_snapshot_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_disk_snapshot_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_disk_snapshot_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_network_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_network_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_network_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_network_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_object_storage_user_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_object_storage_user_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_private_vm_image_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_private_vm_image_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_security_group_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_security_group_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_storage_disk_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_storage_disk_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_storage_disk_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_storage_disk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_vm_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_vm_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
-from src.cudo_compute.configuration import Configuration
+from cudo_compute.configuration import Configuration
 
 
 class CreateVMBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_vm_request_nic.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_vm_request_nic.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/create_vm_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_vm_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/data_center.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/data_center.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/data_center_category.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/data_center_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/data_center_revenue_resource.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/data_center_revenue_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/data_center_time_revenue.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/data_center_time_revenue.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/decimal.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/decimal.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_disk_snapshot_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_disk_snapshot_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_network_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_network_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_object_storage_key_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/delete_object_storage_key_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
-from src.cudo_compute.configuration import Configuration
+from cudo_compute.configuration import Configuration
 
 
 class DeleteObjectStorageKeyResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_object_storage_user_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/delete_object_storage_user_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
-from src.cudo_compute.configuration import Configuration
+from cudo_compute.configuration import Configuration
 
 
 class DeleteObjectStorageUserResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_private_vm_image_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_private_vm_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_security_group_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_security_group_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/delete_storage_disk_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_storage_disk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/detach_security_group_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/detach_security_group_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/detach_storage_disk_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/detach_storage_disk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/disk.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/disk.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
 
@@ -82,15 +83,16 @@
             self.create_time = create_time
         if data_center_id is not None:
             self.data_center_id = data_center_id
         if disk_state is not None:
             self.disk_state = disk_state
         if disk_type is not None:
             self.disk_type = disk_type
-        self.id = id
+        if id is not None:
+            self.id = id
         if private_image_id is not None:
             self.private_image_id = private_image_id
         if project_id is not None:
             self.project_id = project_id
         if public_image_id is not None:
             self.public_image_id = public_image_id
         self.size_gib = size_gib
@@ -197,16 +199,14 @@
     def id(self, id):
         """Sets the id of this Disk.
 
 
         :param id: The id of this Disk.  # noqa: E501
         :type: str
         """
-        if self._configuration.client_side_validation and id is None:
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def private_image_id(self):
         """Gets the private_image_id of this Disk.  # noqa: E501
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/disk_state.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/disk_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/disk_storage_class.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/disk_storage_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/disk_storage_price_hr.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/disk_storage_price_hr.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/disk_type.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/disk_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/generate_api_key_request.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/generate_api_key_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_billing_account_details_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_billing_account_details_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_billing_account_spend_details_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_billing_account_spend_details_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_billing_account_stripe_invoices_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_billing_account_stripe_invoices_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_data_center_live_utilization_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_data_center_live_utilization_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_data_center_revenue_by_resource_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_data_center_revenue_by_resource_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_data_center_revenue_time_series_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_data_center_revenue_time_series_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_disk_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_disk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_machine_type_live_utilization_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_machine_type_live_utilization_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_machine_type_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_machine_type_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_network_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_network_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
-from src.cudo_compute.configuration import Configuration
+from cudo_compute.configuration import Configuration
 
 
 class GetNetworkResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_object_storage_session_key_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_object_storage_session_key_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_private_vm_image_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_private_vm_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_security_group_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_security_group_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/get_vm_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_vm_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/gpu_model_category.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/gpu_model_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/host.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/host.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/host_config_category.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/host_config_category.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/identity_verification_session.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/identity_verification_session.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/image.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/interval.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/invoice.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_api_keys_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_api_keys_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_billing_accounts_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_billing_accounts_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_clusters_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_clusters_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_data_centers_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_data_centers_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_disk_snapshots_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_disk_snapshots_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_disks_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_disks_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_hosts_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_hosts_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_machine_types_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_machine_types_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_networks_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_networks_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_object_storage_buckets_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_object_storage_buckets_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_object_storage_keys_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_object_storage_keys_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_object_storage_users_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_object_storage_users_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_outstanding_stripe_invoices_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_outstanding_stripe_invoices_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_private_vm_images_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_private_vm_images_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_private_vm_images_response_private_image.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_private_vm_images_response_private_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_project_ssh_keys_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_project_ssh_keys_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_projects_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_projects_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_public_vm_images_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_public_vm_images_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_regions_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_regions_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_security_groups_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_security_groups_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_ssh_keys_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_ssh_keys_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_user_permissions_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_user_permissions_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_vm_data_centers_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_vm_data_centers_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_vm_disks_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_vm_disks_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_vm_machine_types_request.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_vm_machine_types_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_vm_machine_types_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_vm_machine_types_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/list_vms_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/list_vms_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/machine_type.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/machine_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/monitor_vm_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/monitor_vm_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/network.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/network_price_hr.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/network_price_hr.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/network_state.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/network_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/object_storage_bucket.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/object_storage_bucket.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/object_storage_key.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/object_storage_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/object_storage_user.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/object_storage_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/payment_method_card.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/payment_method_card.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/payment_method_paypal.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/payment_method_paypal.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/point.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/point.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/profile.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/project.py` & `cudo_compute-0.1.8/out/cudo_compute/models/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
-from src.cudo_compute.configuration import Configuration
+from cudo_compute.configuration import Configuration
 
 
 class Project(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/protocol.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/reboot_vm_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/reboot_vm_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/region.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/remove_billing_account_payment_method_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/remove_billing_account_payment_method_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/remove_billing_account_user_permission_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/remove_billing_account_user_permission_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/remove_data_center_user_permission_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/remove_data_center_user_permission_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/remove_project_user_permission_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/remove_project_user_permission_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/resize_vm_disk_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/resize_vm_disk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/resize_vm_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/resize_vm_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/revert_disk_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/revert_disk_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
-from src.cudo_compute.configuration import Configuration
+from cudo_compute.configuration import Configuration
 
 
 class RevertDiskResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/role.py` & `cudo_compute-0.1.8/out/cudo_compute/models/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
-from src.cudo_compute.configuration import Configuration
+from cudo_compute.configuration import Configuration
 
 
 class Role(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/rule.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/rule_type.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/rule_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/security_group.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/security_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/security_group1.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/security_group1.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/security_group_rule.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/security_group_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/set_billing_account_default_payment_method_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/set_billing_account_default_payment_method_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/snapshot.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/snapshot.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/ssh_key.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/ssh_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/ssh_key_source.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/ssh_key_source.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/start_network_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/start_network_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/start_vm_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/start_vm_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/status.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/stop_network_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/stop_network_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/stop_vm_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/revert_disk_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,24 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
-from src.cudo_compute.configuration import Configuration
+from cudo_compute.configuration import Configuration
 
 
-class StopVMResponse(object):
+class RevertDiskResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -34,15 +35,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None):  # noqa: E501
-        """StopVMResponse - a model defined in Swagger"""  # noqa: E501
+        """RevertDiskResponse - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -61,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(StopVMResponse, dict):
+        if issubclass(RevertDiskResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,18 +78,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StopVMResponse):
+        if not isinstance(other, RevertDiskResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, StopVMResponse):
+        if not isinstance(other, RevertDiskResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/stripe_customer.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/stripe_customer.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/tax_id.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/tax_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/terminate_vm_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/terminate_vm_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/unit.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/update_billing_account_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/update_billing_account_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/update_private_vm_image_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/update_private_vm_image_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/update_security_group_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/update_security_group_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/update_vm_metadata_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/update_vm_metadata_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/update_vm_metadata_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/update_vm_metadata_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/user_permission.py` & `cudo_compute-0.1.8/out/cudo_compute/models/user_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
-from src.cudo_compute.configuration import Configuration
+from cudo_compute.configuration import Configuration
 
 
 class UserPermission(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/v1_private_image.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/v1_private_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/v_router_size.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/v_router_size.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/vm.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/vm.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/vm_data_center.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/vm_data_center.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/vm_data_center_storage_class.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/vm_data_center_storage_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/vm_monitoring_item.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/vm_monitoring_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/vm_state.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/vm_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/docs/src/cudo_compute/models/vmnic.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/vmnic.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)  # noqa: E501
 
     OpenAPI spec version: 1.0.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
+
 import pprint
 import re  # noqa: F401
 
 import six
 
 from src.cudo_compute.configuration import Configuration
```

### Comparing `cudo_compute-0.1.7/helpers/auth_config.py` & `cudo_compute-0.1.8/helpers/auth_config.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/helpers/cudo_api.py` & `cudo_compute-0.1.8/helpers/cudo_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/.gitignore` & `cudo_compute-0.1.8/out/.gitignore`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/.swagger-codegen-ignore` & `cudo_compute-0.1.8/out/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/README.md` & `cudo_compute-0.1.8/out/README.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/git_push.sh` & `cudo_compute-0.1.8/out/git_push.sh`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/setup.py` & `cudo_compute-0.1.8/out/setup.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/__init__.py` & `cudo_compute-0.1.8/out/cudo_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api_client.py` & `cudo_compute-0.1.8/out/cudo_compute/api_client.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/configuration.py` & `cudo_compute-0.1.8/out/cudo_compute/configuration.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/rest.py` & `cudo_compute-0.1.8/out/cudo_compute/rest.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/__init__.py` & `cudo_compute-0.1.8/out/cudo_compute/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/api_keys_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/api_keys_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/billing_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/billing_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/data_centers_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/data_centers_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/disks_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/disks_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/machine_types_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/machine_types_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/networks_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/networks_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/object_storage_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/object_storage_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/permissions_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/permissions_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/projects_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/search_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/search_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/ssh_keys_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/ssh_keys_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/user_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/user_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/api/virtual_machines_api.py` & `cudo_compute-0.1.8/out/cudo_compute/api/virtual_machines_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/__init__.py` & `cudo_compute-0.1.8/out/cudo_compute/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/activate_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/activate_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/add_billing_account_user_permission_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/add_billing_account_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/add_data_center_user_permission_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/add_data_center_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/add_project_user_permission_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/add_project_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/any.py` & `cudo_compute-0.1.8/out/cudo_compute/models/any.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/api_key.py` & `cudo_compute-0.1.8/out/cudo_compute/models/api_key.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/attach_security_group_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/attach_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/attach_storage_disk_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/attach_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/billing_account.py` & `cudo_compute-0.1.8/out/cudo_compute/models/billing_account.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/billing_account_payment_method.py` & `cudo_compute-0.1.8/out/cudo_compute/models/billing_account_payment_method.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/billing_account_payment_methods.py` & `cudo_compute-0.1.8/out/cudo_compute/models/billing_account_payment_methods.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/billing_account_setup_intent.py` & `cudo_compute-0.1.8/out/cudo_compute/models/billing_account_setup_intent.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/billing_account_spend_row.py` & `cudo_compute-0.1.8/out/cudo_compute/models/billing_account_spend_row.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/cluster.py` & `cudo_compute-0.1.8/out/cudo_compute/models/cluster.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/connect_vm_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/connect_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/count_hosts_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/count_hosts_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/count_vms_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/count_vms_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/cpu_model_category.py` & `cudo_compute-0.1.8/out/cudo_compute/models/cpu_model_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_billing_account_request.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_billing_account_request.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_disk_snapshot_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_disk_snapshot_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_disk_snapshot_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_disk_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_network_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_network_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_network_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_object_storage_user_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_object_storage_user_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_private_vm_image_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_security_group_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_storage_disk_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_storage_disk_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_storage_disk_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_vm_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_vm_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_vm_request_nic.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_vm_request_nic.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/create_vm_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/create_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/data_center.py` & `cudo_compute-0.1.8/out/cudo_compute/models/data_center.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/data_center_category.py` & `cudo_compute-0.1.8/out/cudo_compute/models/data_center_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/data_center_revenue_resource.py` & `cudo_compute-0.1.8/out/cudo_compute/models/data_center_revenue_resource.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/data_center_time_revenue.py` & `cudo_compute-0.1.8/out/cudo_compute/models/data_center_time_revenue.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/decimal.py` & `cudo_compute-0.1.8/out/cudo_compute/models/decimal.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/delete_disk_snapshot_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/delete_disk_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/delete_network_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/delete_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/delete_object_storage_key_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/delete_object_storage_key_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/delete_object_storage_user_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/delete_object_storage_user_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/delete_private_vm_image_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/delete_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/delete_security_group_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/delete_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/delete_storage_disk_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/delete_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/detach_security_group_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/detach_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/detach_storage_disk_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/detach_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/disk.py` & `cudo_compute-0.1.8/out/cudo_compute/models/disk.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,16 @@
             self.create_time = create_time
         if data_center_id is not None:
             self.data_center_id = data_center_id
         if disk_state is not None:
             self.disk_state = disk_state
         if disk_type is not None:
             self.disk_type = disk_type
-        self.id = id
+        if id is not None:
+            self.id = id
         if private_image_id is not None:
             self.private_image_id = private_image_id
         if project_id is not None:
             self.project_id = project_id
         if public_image_id is not None:
             self.public_image_id = public_image_id
         self.size_gib = size_gib
@@ -198,16 +199,14 @@
     def id(self, id):
         """Sets the id of this Disk.
 
 
         :param id: The id of this Disk.  # noqa: E501
         :type: str
         """
-        if self._configuration.client_side_validation and id is None:
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def private_image_id(self):
         """Gets the private_image_id of this Disk.  # noqa: E501
```

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/disk_state.py` & `cudo_compute-0.1.8/out/cudo_compute/models/disk_state.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/disk_storage_class.py` & `cudo_compute-0.1.8/out/cudo_compute/models/disk_storage_class.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/disk_storage_price_hr.py` & `cudo_compute-0.1.8/out/cudo_compute/models/disk_storage_price_hr.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/disk_type.py` & `cudo_compute-0.1.8/out/cudo_compute/models/disk_type.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/generate_api_key_request.py` & `cudo_compute-0.1.8/out/cudo_compute/models/generate_api_key_request.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_billing_account_details_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_billing_account_details_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_billing_account_spend_details_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_billing_account_spend_details_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_billing_account_stripe_invoices_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_billing_account_stripe_invoices_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_data_center_live_utilization_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_data_center_live_utilization_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_data_center_revenue_by_resource_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_data_center_revenue_by_resource_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_data_center_revenue_time_series_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_data_center_revenue_time_series_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_disk_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_machine_type_live_utilization_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_machine_type_live_utilization_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_machine_type_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_machine_type_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_network_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_object_storage_session_key_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_object_storage_session_key_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_private_vm_image_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_security_group_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/get_vm_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/get_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/gpu_model_category.py` & `cudo_compute-0.1.8/out/cudo_compute/models/gpu_model_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/host.py` & `cudo_compute-0.1.8/out/cudo_compute/models/host.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/host_config_category.py` & `cudo_compute-0.1.8/out/cudo_compute/models/host_config_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/identity_verification_session.py` & `cudo_compute-0.1.8/out/cudo_compute/models/identity_verification_session.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/image.py` & `cudo_compute-0.1.8/out/cudo_compute/models/image.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/interval.py` & `cudo_compute-0.1.8/out/cudo_compute/models/interval.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/invoice.py` & `cudo_compute-0.1.8/out/cudo_compute/models/invoice.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_api_keys_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_billing_accounts_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_billing_accounts_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_clusters_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_clusters_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_data_centers_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_data_centers_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_disk_snapshots_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_disk_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_disks_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_disks_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_hosts_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_hosts_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_machine_types_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_machine_types_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_networks_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_networks_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_object_storage_buckets_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_object_storage_buckets_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_object_storage_keys_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_object_storage_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_object_storage_users_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_object_storage_users_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_outstanding_stripe_invoices_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_outstanding_stripe_invoices_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_private_vm_images_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_private_vm_images_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_private_vm_images_response_private_image.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_private_vm_images_response_private_image.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_project_ssh_keys_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_project_ssh_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_projects_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_projects_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_public_vm_images_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_public_vm_images_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_regions_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_regions_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_security_groups_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_security_groups_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_ssh_keys_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_ssh_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_user_permissions_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_user_permissions_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_vm_data_centers_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_vm_data_centers_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_vm_disks_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_vm_disks_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_vm_machine_types_request.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_vm_machine_types_request.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_vm_machine_types_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_vm_machine_types_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/list_vms_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/list_vms_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/machine_type.py` & `cudo_compute-0.1.8/out/cudo_compute/models/machine_type.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/monitor_vm_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/monitor_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/network.py` & `cudo_compute-0.1.8/out/cudo_compute/models/network.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/network_price_hr.py` & `cudo_compute-0.1.8/out/cudo_compute/models/network_price_hr.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/network_state.py` & `cudo_compute-0.1.8/out/cudo_compute/models/network_state.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/object_storage_bucket.py` & `cudo_compute-0.1.8/out/cudo_compute/models/object_storage_bucket.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/object_storage_key.py` & `cudo_compute-0.1.8/out/cudo_compute/models/object_storage_key.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/object_storage_user.py` & `cudo_compute-0.1.8/out/cudo_compute/models/object_storage_user.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/payment_method_card.py` & `cudo_compute-0.1.8/out/cudo_compute/models/payment_method_card.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/payment_method_paypal.py` & `cudo_compute-0.1.8/out/cudo_compute/models/payment_method_paypal.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/point.py` & `cudo_compute-0.1.8/out/cudo_compute/models/point.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/profile.py` & `cudo_compute-0.1.8/out/cudo_compute/models/profile.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/project.py` & `cudo_compute-0.1.8/src/cudo_compute/models/project.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/protocol.py` & `cudo_compute-0.1.8/out/cudo_compute/models/protocol.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/reboot_vm_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/reboot_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/region.py` & `cudo_compute-0.1.8/out/cudo_compute/models/region.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/remove_billing_account_payment_method_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/remove_billing_account_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/remove_billing_account_user_permission_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/remove_billing_account_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/remove_data_center_user_permission_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/remove_data_center_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/remove_project_user_permission_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/remove_project_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/resize_vm_disk_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/resize_vm_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/resize_vm_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/resize_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/revert_disk_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/revert_disk_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cudo_compute.configuration import Configuration
+from src.cudo_compute.configuration import Configuration
 
 
 class RevertDiskResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/role.py` & `cudo_compute-0.1.8/src/cudo_compute/models/role.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/rule.py` & `cudo_compute-0.1.8/out/cudo_compute/models/rule.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/rule_type.py` & `cudo_compute-0.1.8/out/cudo_compute/models/rule_type.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/security_group.py` & `cudo_compute-0.1.8/out/cudo_compute/models/security_group.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/security_group1.py` & `cudo_compute-0.1.8/out/cudo_compute/models/security_group1.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/security_group_rule.py` & `cudo_compute-0.1.8/out/cudo_compute/models/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/set_billing_account_default_payment_method_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/set_billing_account_default_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/snapshot.py` & `cudo_compute-0.1.8/out/cudo_compute/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/ssh_key.py` & `cudo_compute-0.1.8/out/cudo_compute/models/ssh_key.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/ssh_key_source.py` & `cudo_compute-0.1.8/out/cudo_compute/models/ssh_key_source.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/start_network_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/start_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/start_vm_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/start_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/status.py` & `cudo_compute-0.1.8/out/cudo_compute/models/status.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/stop_network_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/stop_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/stop_vm_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/stop_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/stripe_customer.py` & `cudo_compute-0.1.8/out/cudo_compute/models/stripe_customer.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/tax_id.py` & `cudo_compute-0.1.8/out/cudo_compute/models/tax_id.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/terminate_vm_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/terminate_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/unit.py` & `cudo_compute-0.1.8/out/cudo_compute/models/unit.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/update_billing_account_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/update_billing_account_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/update_private_vm_image_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/update_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/update_security_group_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/update_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/update_vm_metadata_body.py` & `cudo_compute-0.1.8/out/cudo_compute/models/update_vm_metadata_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/update_vm_metadata_response.py` & `cudo_compute-0.1.8/out/cudo_compute/models/update_vm_metadata_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/user_permission.py` & `cudo_compute-0.1.8/src/cudo_compute/models/user_permission.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/v1_private_image.py` & `cudo_compute-0.1.8/out/cudo_compute/models/v1_private_image.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py` & `cudo_compute-0.1.8/out/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/v_router_size.py` & `cudo_compute-0.1.8/out/cudo_compute/models/v_router_size.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/vm.py` & `cudo_compute-0.1.8/out/cudo_compute/models/vm.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/vm_data_center.py` & `cudo_compute-0.1.8/out/cudo_compute/models/vm_data_center.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/vm_data_center_storage_class.py` & `cudo_compute-0.1.8/out/cudo_compute/models/vm_data_center_storage_class.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/vm_monitoring_item.py` & `cudo_compute-0.1.8/out/cudo_compute/models/vm_monitoring_item.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/vm_state.py` & `cudo_compute-0.1.8/out/cudo_compute/models/vm_state.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/cudo_compute/models/vmnic.py` & `cudo_compute-0.1.8/out/cudo_compute/models/vmnic.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/APIKeysApi.md` & `cudo_compute-0.1.8/out/docs/APIKeysApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/BillingAccount.md` & `cudo_compute-0.1.8/out/docs/BillingAccount.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/BillingAccountPaymentMethod.md` & `cudo_compute-0.1.8/out/docs/BillingAccountPaymentMethod.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/BillingAccountSpendRow.md` & `cudo_compute-0.1.8/out/docs/BillingAccountSpendRow.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/BillingApi.md` & `cudo_compute-0.1.8/out/docs/BillingApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/Cluster.md` & `cudo_compute-0.1.8/out/docs/Cluster.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/CreateVMBody.md` & `cudo_compute-0.1.8/out/docs/CreateVMBody.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/DataCenter.md` & `cudo_compute-0.1.8/out/docs/DataCenter.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/DataCentersApi.md` & `cudo_compute-0.1.8/out/docs/DataCentersApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/Decimal.md` & `cudo_compute-0.1.8/out/docs/Decimal.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/Disk.md` & `cudo_compute-0.1.8/out/docs/Disk.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ## Properties
 Name | Type | Description | Notes
 ------------ | ------------- | ------------- | -------------
 **create_time** | **datetime** |  | [optional] 
 **data_center_id** | **str** |  | [optional] 
 **disk_state** | [**DiskState**](DiskState.md) |  | [optional] 
 **disk_type** | [**DiskType**](DiskType.md) |  | [optional] 
-**id** | **str** |  | 
+**id** | **str** |  | [optional] 
 **private_image_id** | **str** |  | [optional] 
 **project_id** | **str** |  | [optional] 
 **public_image_id** | **str** |  | [optional] 
 **size_gib** | **int** |  | 
 **storage_class** | [**DiskStorageClass**](DiskStorageClass.md) |  | [optional] 
 **vm_id** | **str** |  | [optional]
```

### Comparing `cudo_compute-0.1.7/out/docs/DiskStoragePriceHr.md` & `cudo_compute-0.1.8/out/docs/DiskStoragePriceHr.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/DisksApi.md` & `cudo_compute-0.1.8/out/docs/DisksApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/GenerateApiKeyRequest.md` & `cudo_compute-0.1.8/out/docs/GenerateApiKeyRequest.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/GetDataCenterLiveUtilizationResponse.md` & `cudo_compute-0.1.8/out/docs/GetDataCenterLiveUtilizationResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/GetMachineTypeLiveUtilizationResponse.md` & `cudo_compute-0.1.8/out/docs/GetMachineTypeLiveUtilizationResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/GetMachineTypeResponse.md` & `cudo_compute-0.1.8/out/docs/GetMachineTypeResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/GetObjectStorageSessionKeyResponse.md` & `cudo_compute-0.1.8/out/docs/GetObjectStorageSessionKeyResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/Host.md` & `cudo_compute-0.1.8/out/docs/Host.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/HostConfigCategory.md` & `cudo_compute-0.1.8/out/docs/HostConfigCategory.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/Invoice.md` & `cudo_compute-0.1.8/out/docs/Invoice.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/ListPrivateVMImagesResponse.md` & `cudo_compute-0.1.8/out/docs/ListPrivateVMImagesResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/ListPrivateVMImagesResponsePrivateImage.md` & `cudo_compute-0.1.8/out/docs/ListPrivateVMImagesResponsePrivateImage.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/ListUserPermissionsResponse.md` & `cudo_compute-0.1.8/out/docs/ListUserPermissionsResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/ListVMMachineTypesRequest.md` & `cudo_compute-0.1.8/out/docs/ListVMMachineTypesRequest.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/ListVMMachineTypesResponse.md` & `cudo_compute-0.1.8/out/docs/ListVMMachineTypesResponse.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/MachineTypesApi.md` & `cudo_compute-0.1.8/out/docs/MachineTypesApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/Network.md` & `cudo_compute-0.1.8/out/docs/Network.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/NetworksApi.md` & `cudo_compute-0.1.8/out/docs/NetworksApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/ObjectStorageApi.md` & `cudo_compute-0.1.8/out/docs/ObjectStorageApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/ObjectStorageBucket.md` & `cudo_compute-0.1.8/out/docs/ObjectStorageBucket.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/PaymentMethodCard.md` & `cudo_compute-0.1.8/out/docs/PaymentMethodCard.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/PermissionsApi.md` & `cudo_compute-0.1.8/out/docs/PermissionsApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/ProjectsApi.md` & `cudo_compute-0.1.8/out/docs/ProjectsApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/Rule.md` & `cudo_compute-0.1.8/out/docs/Rule.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/SSHKeysApi.md` & `cudo_compute-0.1.8/out/docs/SSHKeysApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/SearchApi.md` & `cudo_compute-0.1.8/out/docs/SearchApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/SecurityGroupRule.md` & `cudo_compute-0.1.8/out/docs/SecurityGroupRule.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/SshKey.md` & `cudo_compute-0.1.8/out/docs/SshKey.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/UserApi.md` & `cudo_compute-0.1.8/out/docs/UserApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/V1billingaccountsbillingAccountIdBillingAccount.md` & `cudo_compute-0.1.8/out/docs/V1billingaccountsbillingAccountIdBillingAccount.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/VM.md` & `cudo_compute-0.1.8/out/docs/VM.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/VMDataCenter.md` & `cudo_compute-0.1.8/out/docs/VMDataCenter.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/VMMonitoringItem.md` & `cudo_compute-0.1.8/out/docs/VMMonitoringItem.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/VMNIC.md` & `cudo_compute-0.1.8/out/docs/VMNIC.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/docs/VirtualMachinesApi.md` & `cudo_compute-0.1.8/out/docs/VirtualMachinesApi.md`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_activate_body.py` & `cudo_compute-0.1.8/out/test/test_activate_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_add_billing_account_user_permission_body.py` & `cudo_compute-0.1.8/out/test/test_add_billing_account_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_add_data_center_user_permission_body.py` & `cudo_compute-0.1.8/out/test/test_add_data_center_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_add_project_user_permission_body.py` & `cudo_compute-0.1.8/out/test/test_add_project_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_any.py` & `cudo_compute-0.1.8/out/test/test_any.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_api_key.py` & `cudo_compute-0.1.8/out/test/test_api_key.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_api_keys_api.py` & `cudo_compute-0.1.8/out/test/test_api_keys_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_attach_security_group_response.py` & `cudo_compute-0.1.8/out/test/test_attach_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_attach_storage_disk_response.py` & `cudo_compute-0.1.8/out/test/test_attach_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_billing_account.py` & `cudo_compute-0.1.8/out/test/test_billing_account.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_billing_account_payment_method.py` & `cudo_compute-0.1.8/out/test/test_billing_account_payment_method.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_billing_account_payment_methods.py` & `cudo_compute-0.1.8/out/test/test_billing_account_payment_methods.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_billing_account_setup_intent.py` & `cudo_compute-0.1.8/out/test/test_billing_account_setup_intent.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_billing_account_spend_row.py` & `cudo_compute-0.1.8/out/test/test_billing_account_spend_row.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_billing_api.py` & `cudo_compute-0.1.8/out/test/test_billing_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_cluster.py` & `cudo_compute-0.1.8/out/test/test_cluster.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_connect_vm_response.py` & `cudo_compute-0.1.8/out/test/test_connect_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_count_hosts_response.py` & `cudo_compute-0.1.8/out/test/test_count_hosts_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_count_vms_response.py` & `cudo_compute-0.1.8/out/test/test_count_vms_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_cpu_model_category.py` & `cudo_compute-0.1.8/out/test/test_cpu_model_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_billing_account_request.py` & `cudo_compute-0.1.8/out/test/test_create_billing_account_request.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_disk_snapshot_body.py` & `cudo_compute-0.1.8/out/test/test_create_disk_snapshot_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_disk_snapshot_response.py` & `cudo_compute-0.1.8/out/test/test_create_disk_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_network_body.py` & `cudo_compute-0.1.8/out/test/test_create_network_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_network_response.py` & `cudo_compute-0.1.8/out/test/test_create_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_object_storage_user_body.py` & `cudo_compute-0.1.8/out/test/test_create_object_storage_user_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_private_vm_image_response.py` & `cudo_compute-0.1.8/out/test/test_create_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_security_group_response.py` & `cudo_compute-0.1.8/out/test/test_create_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_storage_disk_body.py` & `cudo_compute-0.1.8/out/test/test_create_storage_disk_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_storage_disk_response.py` & `cudo_compute-0.1.8/out/test/test_create_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_vm_body.py` & `cudo_compute-0.1.8/out/test/test_create_vm_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_vm_request_nic.py` & `cudo_compute-0.1.8/out/test/test_create_vm_request_nic.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_create_vm_response.py` & `cudo_compute-0.1.8/out/test/test_create_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_data_center.py` & `cudo_compute-0.1.8/out/test/test_data_center.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_data_center_category.py` & `cudo_compute-0.1.8/out/test/test_data_center_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_data_center_revenue_resource.py` & `cudo_compute-0.1.8/out/test/test_data_center_revenue_resource.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_data_center_time_revenue.py` & `cudo_compute-0.1.8/out/test/test_data_center_time_revenue.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_data_centers_api.py` & `cudo_compute-0.1.8/out/test/test_data_centers_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_decimal.py` & `cudo_compute-0.1.8/out/test/test_decimal.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_delete_disk_snapshot_response.py` & `cudo_compute-0.1.8/out/test/test_delete_disk_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_delete_network_response.py` & `cudo_compute-0.1.8/out/test/test_delete_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_delete_object_storage_key_response.py` & `cudo_compute-0.1.8/out/test/test_delete_object_storage_key_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_delete_object_storage_user_response.py` & `cudo_compute-0.1.8/out/test/test_delete_object_storage_user_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_delete_private_vm_image_response.py` & `cudo_compute-0.1.8/out/test/test_delete_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_delete_security_group_response.py` & `cudo_compute-0.1.8/out/test/test_delete_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_delete_storage_disk_response.py` & `cudo_compute-0.1.8/out/test/test_delete_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_detach_security_group_response.py` & `cudo_compute-0.1.8/out/test/test_detach_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_detach_storage_disk_response.py` & `cudo_compute-0.1.8/out/test/test_detach_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_disk.py` & `cudo_compute-0.1.8/out/test/test_disk.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_disk_state.py` & `cudo_compute-0.1.8/out/test/test_disk_state.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_disk_storage_class.py` & `cudo_compute-0.1.8/out/test/test_disk_storage_class.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_disk_storage_price_hr.py` & `cudo_compute-0.1.8/out/test/test_disk_storage_price_hr.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_disk_type.py` & `cudo_compute-0.1.8/out/test/test_disk_type.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_disks_api.py` & `cudo_compute-0.1.8/out/test/test_disks_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_generate_api_key_request.py` & `cudo_compute-0.1.8/out/test/test_generate_api_key_request.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_billing_account_details_response.py` & `cudo_compute-0.1.8/out/test/test_get_billing_account_details_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_billing_account_spend_details_response.py` & `cudo_compute-0.1.8/out/test/test_get_billing_account_spend_details_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_billing_account_stripe_invoices_response.py` & `cudo_compute-0.1.8/out/test/test_get_billing_account_stripe_invoices_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_data_center_live_utilization_response.py` & `cudo_compute-0.1.8/out/test/test_get_data_center_live_utilization_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_data_center_revenue_by_resource_response.py` & `cudo_compute-0.1.8/out/test/test_get_data_center_revenue_by_resource_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_data_center_revenue_time_series_response.py` & `cudo_compute-0.1.8/out/test/test_get_data_center_revenue_time_series_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_disk_response.py` & `cudo_compute-0.1.8/out/test/test_get_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_machine_type_live_utilization_response.py` & `cudo_compute-0.1.8/out/test/test_get_machine_type_live_utilization_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_machine_type_response.py` & `cudo_compute-0.1.8/out/test/test_get_machine_type_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_network_response.py` & `cudo_compute-0.1.8/out/test/test_get_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_object_storage_session_key_response.py` & `cudo_compute-0.1.8/out/test/test_get_object_storage_session_key_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_private_vm_image_response.py` & `cudo_compute-0.1.8/out/test/test_get_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_security_group_response.py` & `cudo_compute-0.1.8/out/test/test_get_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_get_vm_response.py` & `cudo_compute-0.1.8/out/test/test_get_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_gpu_model_category.py` & `cudo_compute-0.1.8/out/test/test_gpu_model_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_host.py` & `cudo_compute-0.1.8/out/test/test_host.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_host_config_category.py` & `cudo_compute-0.1.8/out/test/test_host_config_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_identity_verification_session.py` & `cudo_compute-0.1.8/out/test/test_identity_verification_session.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_image.py` & `cudo_compute-0.1.8/out/test/test_image.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_interval.py` & `cudo_compute-0.1.8/out/test/test_interval.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_invoice.py` & `cudo_compute-0.1.8/out/test/test_invoice.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_api_keys_response.py` & `cudo_compute-0.1.8/out/test/test_list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_billing_accounts_response.py` & `cudo_compute-0.1.8/out/test/test_list_billing_accounts_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_clusters_response.py` & `cudo_compute-0.1.8/out/test/test_list_clusters_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_data_centers_response.py` & `cudo_compute-0.1.8/out/test/test_list_data_centers_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_disk_snapshots_response.py` & `cudo_compute-0.1.8/out/test/test_list_disk_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_disks_response.py` & `cudo_compute-0.1.8/out/test/test_list_disks_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_hosts_response.py` & `cudo_compute-0.1.8/out/test/test_list_hosts_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_machine_types_response.py` & `cudo_compute-0.1.8/out/test/test_list_machine_types_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_networks_response.py` & `cudo_compute-0.1.8/out/test/test_list_networks_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_object_storage_buckets_response.py` & `cudo_compute-0.1.8/out/test/test_list_object_storage_buckets_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_object_storage_keys_response.py` & `cudo_compute-0.1.8/out/test/test_list_object_storage_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_object_storage_users_response.py` & `cudo_compute-0.1.8/out/test/test_list_object_storage_users_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_outstanding_stripe_invoices_response.py` & `cudo_compute-0.1.8/out/test/test_list_outstanding_stripe_invoices_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_private_vm_images_response.py` & `cudo_compute-0.1.8/out/test/test_list_private_vm_images_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_private_vm_images_response_private_image.py` & `cudo_compute-0.1.8/out/test/test_list_private_vm_images_response_private_image.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_project_ssh_keys_response.py` & `cudo_compute-0.1.8/out/test/test_list_project_ssh_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_projects_response.py` & `cudo_compute-0.1.8/out/test/test_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_public_vm_images_response.py` & `cudo_compute-0.1.8/out/test/test_list_public_vm_images_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_regions_response.py` & `cudo_compute-0.1.8/out/test/test_list_regions_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_security_groups_response.py` & `cudo_compute-0.1.8/out/test/test_list_security_groups_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_ssh_keys_response.py` & `cudo_compute-0.1.8/out/test/test_list_ssh_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_user_permissions_response.py` & `cudo_compute-0.1.8/out/test/test_list_user_permissions_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_vm_data_centers_response.py` & `cudo_compute-0.1.8/out/test/test_list_vm_data_centers_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_vm_disks_response.py` & `cudo_compute-0.1.8/out/test/test_list_vm_disks_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_vm_machine_types_request.py` & `cudo_compute-0.1.8/out/test/test_list_vm_machine_types_request.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_vm_machine_types_response.py` & `cudo_compute-0.1.8/out/test/test_list_vm_machine_types_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_list_vms_response.py` & `cudo_compute-0.1.8/out/test/test_list_vms_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_machine_type.py` & `cudo_compute-0.1.8/out/test/test_machine_type.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_machine_types_api.py` & `cudo_compute-0.1.8/out/test/test_machine_types_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_monitor_vm_response.py` & `cudo_compute-0.1.8/out/test/test_monitor_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_network.py` & `cudo_compute-0.1.8/out/test/test_network.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_network_price_hr.py` & `cudo_compute-0.1.8/out/test/test_network_price_hr.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_network_state.py` & `cudo_compute-0.1.8/out/test/test_network_state.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_networks_api.py` & `cudo_compute-0.1.8/out/test/test_networks_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_object_storage_api.py` & `cudo_compute-0.1.8/out/test/test_object_storage_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_object_storage_bucket.py` & `cudo_compute-0.1.8/out/test/test_object_storage_bucket.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_object_storage_key.py` & `cudo_compute-0.1.8/out/test/test_object_storage_key.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_object_storage_user.py` & `cudo_compute-0.1.8/out/test/test_object_storage_user.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_payment_method_card.py` & `cudo_compute-0.1.8/out/test/test_payment_method_card.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_payment_method_paypal.py` & `cudo_compute-0.1.8/out/test/test_payment_method_paypal.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_permissions_api.py` & `cudo_compute-0.1.8/out/test/test_permissions_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_point.py` & `cudo_compute-0.1.8/out/test/test_point.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_profile.py` & `cudo_compute-0.1.8/out/test/test_profile.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_project.py` & `cudo_compute-0.1.8/out/test/test_project.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_projects_api.py` & `cudo_compute-0.1.8/out/test/test_projects_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_protocol.py` & `cudo_compute-0.1.8/out/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_reboot_vm_response.py` & `cudo_compute-0.1.8/out/test/test_reboot_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_region.py` & `cudo_compute-0.1.8/out/test/test_region.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_remove_billing_account_payment_method_response.py` & `cudo_compute-0.1.8/out/test/test_remove_billing_account_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_remove_billing_account_user_permission_body.py` & `cudo_compute-0.1.8/out/test/test_remove_billing_account_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_remove_data_center_user_permission_body.py` & `cudo_compute-0.1.8/out/test/test_remove_data_center_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_remove_project_user_permission_body.py` & `cudo_compute-0.1.8/out/test/test_remove_project_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_resize_vm_disk_response.py` & `cudo_compute-0.1.8/out/test/test_resize_vm_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_resize_vm_response.py` & `cudo_compute-0.1.8/out/test/test_resize_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_revert_disk_response.py` & `cudo_compute-0.1.8/out/test/test_revert_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_role.py` & `cudo_compute-0.1.8/out/test/test_role.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_rule.py` & `cudo_compute-0.1.8/out/test/test_rule.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_rule_type.py` & `cudo_compute-0.1.8/out/test/test_rule_type.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_search_api.py` & `cudo_compute-0.1.8/out/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_security_group.py` & `cudo_compute-0.1.8/out/test/test_security_group.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_security_group1.py` & `cudo_compute-0.1.8/out/test/test_security_group1.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_security_group_rule.py` & `cudo_compute-0.1.8/out/test/test_security_group_rule.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_set_billing_account_default_payment_method_response.py` & `cudo_compute-0.1.8/out/test/test_set_billing_account_default_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_snapshot.py` & `cudo_compute-0.1.8/out/test/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_ssh_key.py` & `cudo_compute-0.1.8/out/test/test_ssh_key.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_ssh_key_source.py` & `cudo_compute-0.1.8/out/test/test_ssh_key_source.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_ssh_keys_api.py` & `cudo_compute-0.1.8/out/test/test_ssh_keys_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_start_network_response.py` & `cudo_compute-0.1.8/out/test/test_start_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_start_vm_response.py` & `cudo_compute-0.1.8/out/test/test_start_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_status.py` & `cudo_compute-0.1.8/out/test/test_status.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_stop_network_response.py` & `cudo_compute-0.1.8/out/test/test_stop_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_stop_vm_response.py` & `cudo_compute-0.1.8/out/test/test_stop_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_stripe_customer.py` & `cudo_compute-0.1.8/out/test/test_stripe_customer.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_tax_id.py` & `cudo_compute-0.1.8/out/test/test_tax_id.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_terminate_vm_response.py` & `cudo_compute-0.1.8/out/test/test_terminate_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_unit.py` & `cudo_compute-0.1.8/out/test/test_unit.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_update_billing_account_body.py` & `cudo_compute-0.1.8/out/test/test_update_billing_account_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_update_private_vm_image_response.py` & `cudo_compute-0.1.8/out/test/test_update_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_update_security_group_response.py` & `cudo_compute-0.1.8/out/test/test_update_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_update_vm_metadata_body.py` & `cudo_compute-0.1.8/out/test/test_update_vm_metadata_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_update_vm_metadata_response.py` & `cudo_compute-0.1.8/out/test/test_update_vm_metadata_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_user_api.py` & `cudo_compute-0.1.8/out/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_user_permission.py` & `cudo_compute-0.1.8/out/test/test_user_permission.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_v1_private_image.py` & `cudo_compute-0.1.8/out/test/test_v1_private_image.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_v1billingaccountsbilling_account_id_billing_account.py` & `cudo_compute-0.1.8/out/test/test_v1billingaccountsbilling_account_id_billing_account.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_v_router_size.py` & `cudo_compute-0.1.8/out/test/test_v_router_size.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_virtual_machines_api.py` & `cudo_compute-0.1.8/out/test/test_virtual_machines_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_vm.py` & `cudo_compute-0.1.8/out/test/test_vm.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_vm_data_center.py` & `cudo_compute-0.1.8/out/test/test_vm_data_center.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_vm_data_center_storage_class.py` & `cudo_compute-0.1.8/out/test/test_vm_data_center_storage_class.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_vm_monitoring_item.py` & `cudo_compute-0.1.8/out/test/test_vm_monitoring_item.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_vm_state.py` & `cudo_compute-0.1.8/out/test/test_vm_state.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/out/test/test_vmnic.py` & `cudo_compute-0.1.8/out/test/test_vmnic.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/__init__.py` & `cudo_compute-0.1.8/src/cudo_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api_client.py` & `cudo_compute-0.1.8/src/cudo_compute/api_client.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/auth_config.py` & `cudo_compute-0.1.8/src/cudo_compute/auth_config.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/configuration.py` & `cudo_compute-0.1.8/src/cudo_compute/configuration.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/cudo_api.py` & `cudo_compute-0.1.8/src/cudo_compute/cudo_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/rest.py` & `cudo_compute-0.1.8/src/cudo_compute/rest.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/__init__.py` & `cudo_compute-0.1.8/src/cudo_compute/api/__init__.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/api_keys_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/api_keys_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/billing_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/billing_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/data_centers_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/data_centers_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/disks_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/disks_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/machine_types_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/machine_types_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/networks_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/networks_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/object_storage_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/object_storage_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/permissions_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/permissions_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/projects_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/search_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/search_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/ssh_keys_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/ssh_keys_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/user_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/user_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/api/virtual_machines_api.py` & `cudo_compute-0.1.8/src/cudo_compute/api/virtual_machines_api.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/__init__.py` & `cudo_compute-0.1.8/src/cudo_compute/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/activate_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/activate_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/add_billing_account_user_permission_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/add_billing_account_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/add_data_center_user_permission_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/add_data_center_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/add_project_user_permission_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/add_project_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/any.py` & `cudo_compute-0.1.8/src/cudo_compute/models/any.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/api_key.py` & `cudo_compute-0.1.8/src/cudo_compute/models/api_key.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/attach_security_group_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/attach_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/attach_storage_disk_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/attach_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/billing_account.py` & `cudo_compute-0.1.8/src/cudo_compute/models/billing_account.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/billing_account_payment_method.py` & `cudo_compute-0.1.8/src/cudo_compute/models/billing_account_payment_method.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/billing_account_payment_methods.py` & `cudo_compute-0.1.8/src/cudo_compute/models/billing_account_payment_methods.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/billing_account_setup_intent.py` & `cudo_compute-0.1.8/src/cudo_compute/models/billing_account_setup_intent.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/billing_account_spend_row.py` & `cudo_compute-0.1.8/src/cudo_compute/models/billing_account_spend_row.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/cluster.py` & `cudo_compute-0.1.8/src/cudo_compute/models/cluster.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/connect_vm_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/connect_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/count_hosts_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/count_hosts_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/count_vms_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/count_vms_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/cpu_model_category.py` & `cudo_compute-0.1.8/src/cudo_compute/models/cpu_model_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_billing_account_request.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_billing_account_request.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_disk_snapshot_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_disk_snapshot_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_disk_snapshot_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_disk_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_network_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_network_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_network_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_object_storage_user_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_object_storage_user_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_private_vm_image_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_security_group_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_storage_disk_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_storage_disk_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_storage_disk_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_vm_body.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/create_vm_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cudo_compute.configuration import Configuration
+from src.cudo_compute.configuration import Configuration
 
 
 class CreateVMBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_vm_request_nic.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_vm_request_nic.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/create_vm_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/create_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/data_center.py` & `cudo_compute-0.1.8/src/cudo_compute/models/data_center.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/data_center_category.py` & `cudo_compute-0.1.8/src/cudo_compute/models/data_center_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/data_center_revenue_resource.py` & `cudo_compute-0.1.8/src/cudo_compute/models/data_center_revenue_resource.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/data_center_time_revenue.py` & `cudo_compute-0.1.8/src/cudo_compute/models/data_center_time_revenue.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/decimal.py` & `cudo_compute-0.1.8/src/cudo_compute/models/decimal.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/delete_disk_snapshot_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/delete_disk_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/delete_network_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/delete_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/delete_object_storage_key_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_object_storage_key_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cudo_compute.configuration import Configuration
+from src.cudo_compute.configuration import Configuration
 
 
 class DeleteObjectStorageKeyResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/delete_object_storage_user_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/delete_object_storage_user_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cudo_compute.configuration import Configuration
+from src.cudo_compute.configuration import Configuration
 
 
 class DeleteObjectStorageUserResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/delete_private_vm_image_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/delete_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/delete_security_group_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/delete_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/delete_storage_disk_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/delete_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/detach_security_group_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/detach_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/detach_storage_disk_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/detach_storage_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/disk.py` & `cudo_compute-0.1.8/src/cudo_compute/models/disk.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,16 @@
             self.create_time = create_time
         if data_center_id is not None:
             self.data_center_id = data_center_id
         if disk_state is not None:
             self.disk_state = disk_state
         if disk_type is not None:
             self.disk_type = disk_type
-        self.id = id
+        if id is not None:
+            self.id = id
         if private_image_id is not None:
             self.private_image_id = private_image_id
         if project_id is not None:
             self.project_id = project_id
         if public_image_id is not None:
             self.public_image_id = public_image_id
         self.size_gib = size_gib
@@ -198,16 +199,14 @@
     def id(self, id):
         """Sets the id of this Disk.
 
 
         :param id: The id of this Disk.  # noqa: E501
         :type: str
         """
-        if self._configuration.client_side_validation and id is None:
-            raise ValueError("Invalid value for `id`, must not be `None`")  # noqa: E501
 
         self._id = id
 
     @property
     def private_image_id(self):
         """Gets the private_image_id of this Disk.  # noqa: E501
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/disk_state.py` & `cudo_compute-0.1.8/src/cudo_compute/models/disk_state.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/disk_storage_class.py` & `cudo_compute-0.1.8/src/cudo_compute/models/disk_storage_class.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/disk_storage_price_hr.py` & `cudo_compute-0.1.8/src/cudo_compute/models/disk_storage_price_hr.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/disk_type.py` & `cudo_compute-0.1.8/src/cudo_compute/models/disk_type.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/generate_api_key_request.py` & `cudo_compute-0.1.8/src/cudo_compute/models/generate_api_key_request.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_billing_account_details_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_billing_account_details_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_billing_account_spend_details_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_billing_account_spend_details_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_billing_account_stripe_invoices_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_billing_account_stripe_invoices_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_data_center_live_utilization_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_data_center_live_utilization_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_data_center_revenue_by_resource_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_data_center_revenue_by_resource_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_data_center_revenue_time_series_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_data_center_revenue_time_series_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_disk_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_machine_type_live_utilization_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_machine_type_live_utilization_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_machine_type_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_machine_type_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_network_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/get_network_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cudo_compute.configuration import Configuration
+from src.cudo_compute.configuration import Configuration
 
 
 class GetNetworkResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_object_storage_session_key_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_object_storage_session_key_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_private_vm_image_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_security_group_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/get_vm_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/get_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/gpu_model_category.py` & `cudo_compute-0.1.8/src/cudo_compute/models/gpu_model_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/host.py` & `cudo_compute-0.1.8/src/cudo_compute/models/host.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/host_config_category.py` & `cudo_compute-0.1.8/src/cudo_compute/models/host_config_category.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/identity_verification_session.py` & `cudo_compute-0.1.8/src/cudo_compute/models/identity_verification_session.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/image.py` & `cudo_compute-0.1.8/src/cudo_compute/models/image.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/interval.py` & `cudo_compute-0.1.8/src/cudo_compute/models/interval.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/invoice.py` & `cudo_compute-0.1.8/src/cudo_compute/models/invoice.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_api_keys_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_billing_accounts_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_billing_accounts_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_clusters_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_clusters_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_data_centers_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_data_centers_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_disk_snapshots_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_disk_snapshots_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_disks_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_disks_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_hosts_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_hosts_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_machine_types_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_machine_types_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_networks_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_networks_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_object_storage_buckets_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_object_storage_buckets_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_object_storage_keys_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_object_storage_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_object_storage_users_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_object_storage_users_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_outstanding_stripe_invoices_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_outstanding_stripe_invoices_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_private_vm_images_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_private_vm_images_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_private_vm_images_response_private_image.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_private_vm_images_response_private_image.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_project_ssh_keys_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_project_ssh_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_projects_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_projects_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_public_vm_images_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_public_vm_images_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_regions_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_regions_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_security_groups_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_security_groups_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_ssh_keys_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_ssh_keys_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_user_permissions_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_user_permissions_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_vm_data_centers_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_vm_data_centers_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_vm_disks_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_vm_disks_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_vm_machine_types_request.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_vm_machine_types_request.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_vm_machine_types_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_vm_machine_types_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/list_vms_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/list_vms_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/machine_type.py` & `cudo_compute-0.1.8/src/cudo_compute/models/machine_type.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/monitor_vm_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/monitor_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/network.py` & `cudo_compute-0.1.8/src/cudo_compute/models/network.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/network_price_hr.py` & `cudo_compute-0.1.8/src/cudo_compute/models/network_price_hr.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/network_state.py` & `cudo_compute-0.1.8/src/cudo_compute/models/network_state.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/object_storage_bucket.py` & `cudo_compute-0.1.8/src/cudo_compute/models/object_storage_bucket.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/object_storage_key.py` & `cudo_compute-0.1.8/src/cudo_compute/models/object_storage_key.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/object_storage_user.py` & `cudo_compute-0.1.8/src/cudo_compute/models/object_storage_user.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/payment_method_card.py` & `cudo_compute-0.1.8/src/cudo_compute/models/payment_method_card.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/payment_method_paypal.py` & `cudo_compute-0.1.8/src/cudo_compute/models/payment_method_paypal.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/point.py` & `cudo_compute-0.1.8/src/cudo_compute/models/point.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/profile.py` & `cudo_compute-0.1.8/src/cudo_compute/models/profile.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/project.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cudo_compute.configuration import Configuration
+from src.cudo_compute.configuration import Configuration
 
 
 class Project(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/protocol.py` & `cudo_compute-0.1.8/src/cudo_compute/models/protocol.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/reboot_vm_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/reboot_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/region.py` & `cudo_compute-0.1.8/src/cudo_compute/models/region.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/remove_billing_account_payment_method_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/remove_billing_account_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/remove_billing_account_user_permission_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/remove_billing_account_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/remove_data_center_user_permission_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/remove_data_center_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/remove_project_user_permission_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/remove_project_user_permission_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/resize_vm_disk_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/resize_vm_disk_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/resize_vm_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/resize_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/revert_disk_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/stop_network_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import re  # noqa: F401
 
 import six
 
 from cudo_compute.configuration import Configuration
 
 
-class RevertDiskResponse(object):
+class StopNetworkResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -35,15 +35,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None):  # noqa: E501
-        """RevertDiskResponse - a model defined in Swagger"""  # noqa: E501
+        """StopNetworkResponse - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -62,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RevertDiskResponse, dict):
+        if issubclass(StopNetworkResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,18 +78,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RevertDiskResponse):
+        if not isinstance(other, StopNetworkResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, RevertDiskResponse):
+        if not isinstance(other, StopNetworkResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/role.py` & `cudo_compute-0.1.8/src/cudo_compute/models/unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,27 +15,26 @@
 import re  # noqa: F401
 
 import six
 
 from cudo_compute.configuration import Configuration
 
 
-class Role(object):
+class Unit(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNKNOWN = "UNKNOWN"
-    OWNER = "OWNER"
-    VIEWER = "VIEWER"
-    EDITOR = "EDITOR"
+    UNKNOWN = "UNIT_UNKNOWN"
+    GIB_HOUR = "UNIT_GIB_HOUR"
+    HOUR = "UNIT_HOUR"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -43,15 +42,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None):  # noqa: E501
-        """Role - a model defined in Swagger"""  # noqa: E501
+        """Unit - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -70,15 +69,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Role, dict):
+        if issubclass(Unit, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -86,18 +85,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Role):
+        if not isinstance(other, Unit):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Role):
+        if not isinstance(other, Unit):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/rule.py` & `cudo_compute-0.1.8/src/cudo_compute/models/rule.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/rule_type.py` & `cudo_compute-0.1.8/src/cudo_compute/models/rule_type.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/security_group.py` & `cudo_compute-0.1.8/src/cudo_compute/models/security_group.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/security_group1.py` & `cudo_compute-0.1.8/src/cudo_compute/models/security_group1.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/security_group_rule.py` & `cudo_compute-0.1.8/src/cudo_compute/models/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/set_billing_account_default_payment_method_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/set_billing_account_default_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/snapshot.py` & `cudo_compute-0.1.8/src/cudo_compute/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/ssh_key.py` & `cudo_compute-0.1.8/src/cudo_compute/models/ssh_key.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/ssh_key_source.py` & `cudo_compute-0.1.8/src/cudo_compute/models/ssh_key_source.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/start_network_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/start_network_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/start_vm_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/start_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/status.py` & `cudo_compute-0.1.8/src/cudo_compute/models/status.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/stop_network_response.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/stop_vm_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cudo_compute.configuration import Configuration
+from src.cudo_compute.configuration import Configuration
 
 
-class StopNetworkResponse(object):
+class StopVMResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     Attributes:
@@ -35,15 +35,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None):  # noqa: E501
-        """StopNetworkResponse - a model defined in Swagger"""  # noqa: E501
+        """StopVMResponse - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -62,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(StopNetworkResponse, dict):
+        if issubclass(StopVMResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,18 +78,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StopNetworkResponse):
+        if not isinstance(other, StopVMResponse):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, StopNetworkResponse):
+        if not isinstance(other, StopVMResponse):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/stop_vm_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/stop_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/stripe_customer.py` & `cudo_compute-0.1.8/src/cudo_compute/models/stripe_customer.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/tax_id.py` & `cudo_compute-0.1.8/src/cudo_compute/models/tax_id.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/terminate_vm_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/terminate_vm_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/unit.py` & `cudo_compute-0.1.8/src/cudo_compute/models/v_router_size.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,26 +15,27 @@
 import re  # noqa: F401
 
 import six
 
 from cudo_compute.configuration import Configuration
 
 
-class Unit(object):
+class VRouterSize(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNKNOWN = "UNIT_UNKNOWN"
-    GIB_HOUR = "UNIT_GIB_HOUR"
-    HOUR = "UNIT_HOUR"
+    UNKNOWN = "VROUTER_INSTANCE_UNKNOWN"
+    SMALL = "VROUTER_INSTANCE_SMALL"
+    MEDIUM = "VROUTER_INSTANCE_MEDIUM"
+    LARGE = "VROUTER_INSTANCE_LARGE"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -42,15 +43,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None):  # noqa: E501
-        """Unit - a model defined in Swagger"""  # noqa: E501
+        """VRouterSize - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -69,15 +70,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Unit, dict):
+        if issubclass(VRouterSize, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -85,18 +86,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Unit):
+        if not isinstance(other, VRouterSize):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Unit):
+        if not isinstance(other, VRouterSize):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/update_billing_account_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/update_billing_account_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/update_private_vm_image_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/update_private_vm_image_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/update_security_group_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/update_security_group_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/update_vm_metadata_body.py` & `cudo_compute-0.1.8/src/cudo_compute/models/update_vm_metadata_body.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/update_vm_metadata_response.py` & `cudo_compute-0.1.8/src/cudo_compute/models/update_vm_metadata_response.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/user_permission.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/user_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cudo_compute.configuration import Configuration
+from src.cudo_compute.configuration import Configuration
 
 
 class UserPermission(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/v1_private_image.py` & `cudo_compute-0.1.8/src/cudo_compute/models/v1_private_image.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py` & `cudo_compute-0.1.8/src/cudo_compute/models/v1billingaccountsbilling_account_id_billing_account.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/v_router_size.py` & `cudo_compute-0.1.8/src/cudo_compute/models/vm_state.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,27 +15,42 @@
 import re  # noqa: F401
 
 import six
 
 from cudo_compute.configuration import Configuration
 
 
-class VRouterSize(object):
+class VmState(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNKNOWN = "VROUTER_INSTANCE_UNKNOWN"
-    SMALL = "VROUTER_INSTANCE_SMALL"
-    MEDIUM = "VROUTER_INSTANCE_MEDIUM"
-    LARGE = "VROUTER_INSTANCE_LARGE"
+    CLONING = "CLONING"
+    CREATING_SNAPSHOT = "CREATING_SNAPSHOT"
+    DELETED = "DELETED"
+    DELETING = "DELETING"
+    DELETING_SNAPSHOT = "DELETING_SNAPSHOT"
+    FAILED = "FAILED"
+    HOTPLUGGING = "HOTPLUGGING"
+    MIGRATING = "MIGRATING"
+    RECREATING = "RECREATING"
+    REVERTING_SNAPSHOT = "REVERTING_SNAPSHOT"
+    RESIZING = "RESIZING"
+    RESIZING_DISK = "RESIZING_DISK"
+    ACTIVE = "ACTIVE"
+    STARTING = "STARTING"
+    STOPPED = "STOPPED"
+    STOPPING = "STOPPING"
+    SUSPENDED = "SUSPENDED"
+    SUSPENDING = "SUSPENDING"
+    UNKNOWN = "UNKNOWN"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -43,15 +58,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None):  # noqa: E501
-        """VRouterSize - a model defined in Swagger"""  # noqa: E501
+        """VmState - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -70,15 +85,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(VRouterSize, dict):
+        if issubclass(VmState, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -86,18 +101,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, VRouterSize):
+        if not isinstance(other, VmState):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, VRouterSize):
+        if not isinstance(other, VmState):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/vm.py` & `cudo_compute-0.1.8/src/cudo_compute/models/vm.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/vm_data_center.py` & `cudo_compute-0.1.8/src/cudo_compute/models/vm_data_center.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/vm_data_center_storage_class.py` & `cudo_compute-0.1.8/src/cudo_compute/models/vm_data_center_storage_class.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/vm_monitoring_item.py` & `cudo_compute-0.1.8/src/cudo_compute/models/vm_monitoring_item.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/vm_state.py` & `cudo_compute-0.1.8/docs/src/cudo_compute/models/role.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,45 +12,30 @@
 
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from cudo_compute.configuration import Configuration
+from src.cudo_compute.configuration import Configuration
 
 
-class VmState(object):
+class Role(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    CLONING = "CLONING"
-    CREATING_SNAPSHOT = "CREATING_SNAPSHOT"
-    DELETED = "DELETED"
-    DELETING = "DELETING"
-    DELETING_SNAPSHOT = "DELETING_SNAPSHOT"
-    FAILED = "FAILED"
-    HOTPLUGGING = "HOTPLUGGING"
-    MIGRATING = "MIGRATING"
-    RECREATING = "RECREATING"
-    REVERTING_SNAPSHOT = "REVERTING_SNAPSHOT"
-    RESIZING = "RESIZING"
-    RESIZING_DISK = "RESIZING_DISK"
-    ACTIVE = "ACTIVE"
-    STARTING = "STARTING"
-    STOPPED = "STOPPED"
-    STOPPING = "STOPPING"
-    SUSPENDED = "SUSPENDED"
-    SUSPENDING = "SUSPENDING"
     UNKNOWN = "UNKNOWN"
+    OWNER = "OWNER"
+    VIEWER = "VIEWER"
+    EDITOR = "EDITOR"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
@@ -58,15 +43,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self, _configuration=None):  # noqa: E501
-        """VmState - a model defined in Swagger"""  # noqa: E501
+        """Role - a model defined in Swagger"""  # noqa: E501
         if _configuration is None:
             _configuration = Configuration()
         self._configuration = _configuration
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -85,15 +70,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(VmState, dict):
+        if issubclass(Role, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -101,18 +86,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, VmState):
+        if not isinstance(other, Role):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, VmState):
+        if not isinstance(other, Role):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `cudo_compute-0.1.7/src/cudo_compute/models/vmnic.py` & `cudo_compute-0.1.8/src/cudo_compute/models/vmnic.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/swagger/public.swagger.json` & `cudo_compute-0.1.8/swagger/public.swagger.json`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/tools/authfix.py` & `cudo_compute-0.1.8/tools/authfix.py`

 * *Files identical despite different names*

### Comparing `cudo_compute-0.1.7/tools/swaggerfix.py` & `cudo_compute-0.1.8/tools/swaggerfix.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,9 +21,12 @@
 
 instances = find_instances(json_data, "name", "body")
 
 # Print the paths of instances
 for i in instances:
     json_data[i[0]][i[1]][i[2]][i[3]][i[4]]["name"] = json_data[i[0]][i[1]][i[2]]["operationId"] + "Body"
 
+# remove id required
+json_data['definitions']['Disk']['required'] = ['sizeGib']
+
 with open('fix.swagger.json', 'w') as file:
     json.dump(json_data, file, indent=2)
```

### Comparing `cudo_compute-0.1.7/pyproject.toml` & `cudo_compute-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cudo-compute"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
     { name = "Cudo Ventures", email = "dev@cudoventures.com" },
 ]
 description = "A client for cudocompute.com"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `cudo_compute-0.1.7/PKG-INFO` & `cudo_compute-0.1.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: cudo-compute
-Version: 0.1.7
-Summary: A client for cudocompute.com
-Project-URL: Homepage, https://www.cudocompute.com
-Project-URL: Bug Tracker, https://github.com/CudoVentures/cudo-compute-python-client/issues
-Author-email: Cudo Ventures <dev@cudoventures.com>
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Requires-Dist: certifi>=14.05.14
-Requires-Dist: python-dateutil>=2.5.3
-Requires-Dist: ruamel-yaml>=0.17.2
-Requires-Dist: six>=1.10
-Requires-Dist: urllib3>=1.15.1
-Description-Content-Type: text/markdown
-
 # Cudo Compute
 To use this client install cudoctl and run ``./cudoctl init`` follow the steps to enter your API key and choose your project.  
 
 Then when you call cudo_api in python it will grab your API key from the yaml file created by cudoctl.
 
 ```bash
 pip install cudo-compute
@@ -28,15 +10,15 @@
 ```python
 from cudo_compute import cudo_api
 
 api = cudo_api.virtual_machines()
 vms = api.list_vms(cudo_api.project_id())
 ```
 
-A more complete example of various api calls can be seen in the example in ``examples/example.py`` demonstrates how to use it. 
+More examples of various api calls can be found in ``examples``. 
 
 
 
 # Advanced Users / Development
 The code is generated by swagger codegen cli.
 
 Most code is generated in github actions see .github/workflows the generated code is put into a /src/cudo_compute directory
```

