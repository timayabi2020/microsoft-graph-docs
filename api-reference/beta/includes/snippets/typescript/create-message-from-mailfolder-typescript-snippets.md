---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Message = {
	receivedDateTime : new Date("2016-10-19T10:37:00Z"),
	sentDateTime : new Date("2016-10-19T10:37:00Z"),
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