---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : UpdateAlertsPostRequestBody = {
	value : [
		{
			assignedTo : "String",
			closedDateTime : new Date("String (timestamp)"),
			comments : [
				"String",
			],
			feedback : {
				additionalData : {
					"@odata.type" : "microsoft.graph.alertFeedback",
				},
			},
			id : "String (identifier)",
			status : {
				additionalData : {
					"@odata.type" : "microsoft.graph.alertStatus",
				},
			},
			tags : [
				"String",
			],
			vendorInformation : {
				provider : "String",
				vendor : "String",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.security.alerts.updateAlerts.post(requestBody);
}


```