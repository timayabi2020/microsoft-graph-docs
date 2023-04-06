---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChangePasswordPostRequestBody = {
	currentPassword : "xWwvJ]6NMw+bWH-d",
	newPassword : "0eM85N54wFxWwvJ]",
};

const result = async () => {
	await graphServiceClient.me.changePassword.post(requestBody);
}


```