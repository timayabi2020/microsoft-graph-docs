---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ClearPresencePostRequestBody = {
	sessionId : "22553876-f5ab-4529-bffb-cfe50aa89f87",
};

const result = async () => {
	await graphServiceClient.usersById("user-id").presence.clearPresence.post(requestBody);
}


```