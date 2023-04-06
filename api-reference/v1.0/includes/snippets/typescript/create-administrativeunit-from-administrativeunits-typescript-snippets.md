---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AdministrativeUnit = {
	displayName : "Seattle District Technical Schools",
	description : "Seattle district technical schools administration",
	visibility : "HiddenMembership",
};

const result = async () => {
	await graphServiceClient.directory.administrativeUnits.post(requestBody);
}


```