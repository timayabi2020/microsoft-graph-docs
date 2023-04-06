---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Message = {
	subject : "subject-value",
	body : {
		contentType : BodyType.Text,
		content : "content-value",
	},
	inferenceClassification : InferenceClassificationType.Other,
};

const result = async () => {
	await graphServiceClient.me.messagesById("message-id").patch(requestBody);
}


```