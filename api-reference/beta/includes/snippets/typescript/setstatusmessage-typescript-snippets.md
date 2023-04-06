---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SetStatusMessagePostRequestBody = {
	statusMessage : {
		message : {
			content : "Hey I'm currently in a meeting.",
			contentType : BodyType.Text,
		},
		expiryDateTime : {
			dateTime : "2022-10-18T17:05:33.2079781",
			timeZone : "Pacific Standard Time",
		},
	},
};

const result = async () => {
	await graphServiceClient.usersById("user-id").presence.setStatusMessage.post(requestBody);
}


```