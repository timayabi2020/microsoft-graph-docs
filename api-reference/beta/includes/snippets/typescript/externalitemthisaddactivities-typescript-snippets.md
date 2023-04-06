---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AddActivitiesPostRequestBody = {
	activities : [
		{
			"@odata.type" : "#microsoft.graph.externalConnectors.externalActivity",
			type : ExternalActivityType.String,
			startDateTime : new Date("String (timestamp)"),
		},
	],
};

const result = async () => {
	await graphServiceClient.connectionsById("externalConnection-id").itemsById("externalItem-id").externalConnectorsAddActivities.post(requestBody);
}


```