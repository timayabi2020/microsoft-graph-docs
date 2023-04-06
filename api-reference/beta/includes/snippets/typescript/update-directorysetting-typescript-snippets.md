---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : DirectorySetting = {
	values : [
		{
			name : "CustomBlockedWordsList",
			value : "Contoso",
		},
	],
};

const result = async () => {
	await graphServiceClient.settingsById("directorySetting-id").patch(requestBody);
}


```