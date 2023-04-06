---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "Subject eq 'welcome' and importance eq 'normal'",
		orderby: ["subject","importance","receivedDateTime desc"],
	}
};

const result = async () => {
	await graphServiceClient.me.messages.get(configuration);
}


```