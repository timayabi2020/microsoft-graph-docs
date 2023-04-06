---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GetSharedUseLicenseUsageReportPostRequestBody = {
	reportName : CloudPcReportName.SharedUseLicenseUsageReport,
	filter : "ServicePlanId eq '2d1d344e-d10c-41bb-953b-b3a47521dca0' and DateTimeUTC gt datetime'2022-11-30'",
	select : [
		"ServicePlanId",
		"LicenseCount",
		"ClaimedLicenseCount",
		"DateTimeUTC",
	],
	skip : 0,
	top : 100,
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.reports.getSharedUseLicenseUsageReport.post(requestBody);
}


```