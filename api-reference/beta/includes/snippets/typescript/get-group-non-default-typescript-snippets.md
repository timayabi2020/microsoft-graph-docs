---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["allowExternalSenders","autoSubscribeNewMembers","isSubscribedByMail","unseenCount"],
	}
};

const result = async () => {
	await graphServiceClient.groupsById("group-id").get(configuration);
}


```