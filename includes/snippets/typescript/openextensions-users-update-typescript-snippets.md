---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Extension = {
	additionalData : {
		"theme" : "light",
		"color" : "yellow",
		"lang" : "Swahili",
	},
};

const result = async () => {
	await graphServiceClient.me.extensionsById("extension-id").patch(requestBody);
}


```