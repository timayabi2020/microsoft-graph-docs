---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Settings = {
	deletedUserPersonalSiteRetentionPeriodInDays : 365,
	excludedFileExtensionsForSyncApp : [
		".mp3",
	],
	imageTaggingOption : ImageTaggingChoice.Enhanced,
	isLegacyAuthProtocolsEnabled : true,
	isSitesStorageLimitAutomatic : false,
	isSyncButtonHiddenOnPersonalSite : false,
	isUnmanagedSyncAppForTenantRestricted : false,
	personalSiteDefaultStorageLimitInMB : 120000,
};

const result = async () => {
	await graphServiceClient.admin.sharepoint.settings.patch(requestBody);
}


```