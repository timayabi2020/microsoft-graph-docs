---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TeamsTab = {
	displayName : "My Contoso Tab - updated again",
};

const result = async () => {
	await graphServiceClient.chatsById("chat-id").tabsById("teamsTab-id").patch(requestBody);
}


```