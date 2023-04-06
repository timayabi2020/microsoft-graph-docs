---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Alert = {
	assignedTo : "String",
	closedDateTime : new Date("String (timestamp)"),
	comments : [
		"String",
	],
	feedback : AlertFeedback.@odata.type: microsoft.graph.alertFeedback,
	status : AlertStatus.@odata.type: microsoft.graph.alertStatus,
	tags : [
		"String",
	],
	vendorInformation : {
		provider : "String",
		vendor : "String",
	},
};

const result = async () => {
	await graphServiceClient.security.alertsById("alert-id").patch(requestBody);
}


```