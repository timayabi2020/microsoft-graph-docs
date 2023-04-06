---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AppRoleAssignment = {
	principalId : "cde330e5-2150-4c11-9c5b-14bfdc948c79",
	resourceId : "8e881353-1735-45af-af21-ee1344582a4d",
	appRoleId : "00000000-0000-0000-0000-000000000000",
};

const result = async () => {
	await graphServiceClient.usersById("user-id").appRoleAssignments.post(requestBody);
}


```