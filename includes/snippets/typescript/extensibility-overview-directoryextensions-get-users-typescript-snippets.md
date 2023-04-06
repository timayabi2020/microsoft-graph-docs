---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["id","displayName","extension_b7d8e648520f41d3b9c0fdeb91768a0a_jobGroupTracker","extension_b7d8e648520f41d3b9c0fdeb91768a0a_permanent_pensionable"],
	}
};

const result = async () => {
	await graphServiceClient.users.get(configuration);
}


```