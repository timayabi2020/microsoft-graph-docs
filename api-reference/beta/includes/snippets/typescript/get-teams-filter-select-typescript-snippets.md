---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "displayName eq 'A Contoso Team'",
		select: ["id","description"],
	}
};

async () => {
	await graphServiceClient.teams.get(configuration);
}


```