---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GetRemoteConnectionHistoricalReportsPostRequestBody = {
	filter : "CloudPcId eq '40f9315c-5b63-4126-9f89-b7dcb14fffff' and SignInDateTime gt datetime'2022-09-09T01:22:51.849Z'",
	select : [
		"SignInDateTime",
		"SignOutDateTime",
		"UsageInHour",
		"RoundTripTimeInMsP50",
		"AvailableBandwidthInMBpsP50",
		"RemoteSignInTimeInSec",
	],
	top : 25,
	skip : 0,
};

const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.reports.getRemoteConnectionHistoricalReports.post(requestBody);
}


```