---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "isElevated eq true and expirationDateTime ne null or isElevated eq false",
	}
};

const result = async () => {
	await graphServiceClient.privilegedRoleAssignments.get(configuration);
}


```