---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "displayName eq 'Microsoft Graph'",
		select: ["id","displayName","appId","appRoles"],
	}
};

const result = async () => {
	await graphServiceClient.servicePrincipals.get(configuration);
}


```