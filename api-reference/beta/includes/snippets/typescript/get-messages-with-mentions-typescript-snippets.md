---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "MentionsPreview/IsMentioned eq true",
		select: ["Subject","Sender","ReceivedDateTime","MentionsPreview"],
	}
};

const result = async () => {
	await graphServiceClient.me.messages.get(configuration);
}


```