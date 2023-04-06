---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Channel = {
	displayName : "Import_150958_99z",
	description : "Import_150958_99z",
	createdDateTime : new Date("2020-03-14T11:22:17.067Z"),
	additionalData : {
		"@microsoft.graph.channelCreationMode" : "migration",
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channels.post(requestBody);
}


```