---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GetTotalAggregatedRemoteConnectionReportsPostRequestBody = {
	top : 25,
	skip : 0,
	filter : "(TotalUsageInHour ge 40 and TotalUsageInHour le 80)",
	select : [
		"CloudPcId",
		"ManagedDeviceName",
		"UserPrincipalName",
		"TotalUsageInHour",
		"DaysSinceLastSignIn",
	],
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.reports.getTotalAggregatedRemoteConnectionReports.post(requestBody);
}


```