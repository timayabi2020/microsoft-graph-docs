---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		select: ["name","description","id","scenarios"],
		filter: "scenarios has 'secureFoundation'",
	}
};

const result = async () => {
	await graphServiceClient.identity.conditionalAccess.templates.get(configuration);
}


```