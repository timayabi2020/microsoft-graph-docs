---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MovePostRequestBody = {
	destinationId : "destinationId-value",
};

const result = async () => {
	await graphServiceClient.me.mailFoldersById("mailFolder-id").move.post(requestBody);
}


```