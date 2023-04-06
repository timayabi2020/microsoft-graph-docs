---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Message = {
	receivedDateTime : new Date("datetime-value"),
	sentDateTime : new Date("datetime-value"),
	hasAttachments : true,
	subject : "subject-value",
	body : {
		contentType : BodyType.Text,
		content : "content-value",
	},
	bodyPreview : "bodyPreview-value",
};

const result = async () => {
	await graphServiceClient.me.mailFoldersById("mailFolder-id").messages.post(requestBody);
}


```