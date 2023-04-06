---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		filter: "resourceId eq 8e881353-1735-45af-af21-ee1344582a4d",
	}
};

const result = async () => {
	await graphServiceClient.usersById("user-id").appRoleAssignments.get(configuration);
}


```