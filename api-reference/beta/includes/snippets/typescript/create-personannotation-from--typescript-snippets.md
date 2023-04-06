---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PersonAnnotation = {
	detail : {
		contentType : BodyType.Text,
		content : "I am originally from Australia, but grew up in Moscow, Russia.",
	},
	displayName : "About Me",
};

const result = async () => {
	await graphServiceClient.me.profile.notes.post(requestBody);
}


```