---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["details"],
	}
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.templatesById("conditionalAccessTemplate-id").get(configuration);
}


```