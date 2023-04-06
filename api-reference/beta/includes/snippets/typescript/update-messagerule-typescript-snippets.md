---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MessageRule = {
	displayName : "Important from partner",
	actions : {
		markImportance : Importance.High,
	},
};

const result = async () => {
	await graphServiceClient.me.mailFoldersById("mailFolder-id").messageRulesById("messageRule-id").patch(requestBody);
}


```