---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		expand: ["teamsApp"],
		filter: "teamsApp/id eq 'com.microsoft.teamspace.tab.web'",
	}
};

const result = async () => {
	await graphServiceClient.chatsById("chat-id").tabs.get(configuration);
}


```