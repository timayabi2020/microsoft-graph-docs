---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"ConsistencyLevel": "eventual",
	}
,	queryParameters : {
		count: true,
		select: ["displayName","accountEnabled","servicePrincipalType","signInAudience"],
	}
};

const result = async () => {
	await graphServiceClient.me.appRoleAssignedResources.get(configuration);
}


```