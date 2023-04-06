---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AlertRule = {
	id : "215c55cc-b1c9-4d36-a870-be5778101714",
	displayName : "Azure network connection failure impacting Cloud PCs",
	severity : RuleSeverityType.Informational,
	isSystemRule : true,
	description : "Azure network connection checks have failed and is potentially impacting existing Cloud PCs and blocking the provisioning of new Cloud PCs",
	enabled : true,
	alertRuleTemplate : AlertRuleTemplate.CloudPcOnPremiseNetworkConnectionCheckScenario,
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
	await graphServiceClient.deviceManagement.monitoring.alertRules.post(requestBody);
}


```