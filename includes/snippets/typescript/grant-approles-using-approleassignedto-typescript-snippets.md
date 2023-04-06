---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AppRoleAssignment = {
	principalId : "b0d9b9e3-0ecf-4bfd-8dab-9273dd055a94",
	resourceId : "7ea9e944-71ce-443d-811c-71e8047b557a",
	appRoleId : "df021288-bdef-4463-88db-98f22de89214",
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").appRoleAssignedTo.post(requestBody);
}


```