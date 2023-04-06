---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SetStatusMessagePostRequestBody = {
	statusMessage : {
		message : {
			content : "Hey I am available now",
			contentType : BodyType.Text,
		},
	},
};

const result = async () => {
	await graphServiceClient.usersById("user-id").presence.setStatusMessage.post(requestBody);
}


```