---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CloudPcExportJob = {
	reportName : CloudPcReportName.TotalAggregatedRemoteConnectionReports,
	select : [
		"CloudPcId",
		"ManagedDeviceName",
		"UserPrincipalName",
		"DaysSinceLastSignIn",
		"TotalUsageInHour",
	],
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.reports.exportJobs.post(requestBody);
}


```