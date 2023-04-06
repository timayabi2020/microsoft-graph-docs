---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ItemEmail = {
	displayName : "Business Email",
	type : EmailType.Work,
};

const result = async () => {
	await graphServiceClient.usersById("user-id").profile.emailsById("itemEmail-id").patch(requestBody);
}


```