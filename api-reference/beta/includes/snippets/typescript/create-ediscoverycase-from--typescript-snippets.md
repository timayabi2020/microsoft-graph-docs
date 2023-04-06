---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EdiscoveryCase = {
	displayName : "CONTOSO LITIGATION-005",
	description : "Project Bazooka",
	externalId : "324516",
};

const result = async () => {
	await graphServiceClient.security.cases.ediscoveryCases.post(requestBody);
}


```