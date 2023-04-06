---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "VideoTeleconferenceId eq '123456789'",
	}
};

const result = async () => {
	await graphServiceClient.communications.onlineMeetings.get(configuration);
}


```