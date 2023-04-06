---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AppRoleAssignment = {
	principalId : "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
	principalType : "User",
	appRoleId : "3a84e31e-bffa-470f-b9e6-754a61e4dc63",
	resourceId : "a750f6cf-2319-464a-bcc3-456926736a91",
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").appRoleAssignments.post(requestBody);
}


```