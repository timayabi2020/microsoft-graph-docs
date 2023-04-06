---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SetUserPreferredPresencePostRequestBody = {
	availability : "DoNotDisturb",
	activity : "DoNotDisturb",
	expirationDuration : pT8H,
};

const result = async () => {
	await graphServiceClient.usersById("user-id").presence.setUserPreferredPresence.post(requestBody);
}


```