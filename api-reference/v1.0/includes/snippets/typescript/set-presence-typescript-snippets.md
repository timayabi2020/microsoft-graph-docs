---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SetPresencePostRequestBody = {
	sessionId : "22553876-f5ab-4529-bffb-cfe50aa89f87",
	availability : "Available",
	activity : "Available",
	expirationDuration : pT1H,
};

const result = async () => {
	await graphServiceClient.usersById("user-id").presence.setPresence.post(requestBody);
}


```