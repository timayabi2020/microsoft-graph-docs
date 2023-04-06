---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Team = {
	displayName : "My Class Team",
	description : "My Class Team’s Description",
	additionalData : {
		"template@odata.bind" : "https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')",
	},
};

const result = async () => {
	await graphServiceClient.teams.post(requestBody);
}


```