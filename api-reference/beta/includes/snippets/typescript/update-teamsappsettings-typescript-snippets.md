---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TeamsAppSettings = {
	"@odata.type" : "#microsoft.graph.teamsAppSettings",
	isChatResourceSpecificConsentEnabled : true,
};

const result = async () => {
	await graphServiceClient.teamwork.teamsAppSettings.patch(requestBody);
}


```