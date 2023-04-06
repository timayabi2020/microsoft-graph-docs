---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Permission = {
	roles : [
		"write",
	],
	grantedToIdentities : [
		{
			application : {
				id : "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
				displayName : "Contoso Time Manager App",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.sitesById("site-id").permissions.post(requestBody);
}


```