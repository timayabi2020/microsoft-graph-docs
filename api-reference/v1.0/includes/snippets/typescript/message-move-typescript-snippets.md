---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : MovePostRequestBody = {
	destinationId : "deleteditems",
};

const result = async () => {
	await graphServiceClient.me.messagesById("message-id").move.post(requestBody);
}


```