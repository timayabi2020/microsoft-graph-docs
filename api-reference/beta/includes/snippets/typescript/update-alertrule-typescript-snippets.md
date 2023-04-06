---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AlertRule = {
	severity : RuleSeverityType.Informational,
	enabled : true,
	threshold : {
		aggregation : AggregationType.Count,
		operator : OperatorType.GreaterOrEqual,
		target : 90,
	},
	notificationChannels : [
		{
			notificationChannelType : NotificationChannelType.Portal,
			receivers : [
				"",
			],
			notificationReceivers : [
			],
		},
		{
			notificationChannelType : NotificationChannelType.Email,
			receivers : [
				"serena.davis@contoso.com",
			],
			notificationReceivers : [
				{
					locale : "en-us",
					contactInformation : "serena.davis@contoso.com",
				},
			],
		},
	],
};

const result = async () => {
	await graphServiceClient.deviceManagement.monitoring.alertRulesById("alertRule-id").patch(requestBody);
}


```