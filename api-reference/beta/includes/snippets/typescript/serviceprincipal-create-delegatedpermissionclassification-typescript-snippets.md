---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : DelegatedPermissionClassification = {
	permissionId : "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
	permissionName : "User.Read",
	classification : PermissionClassificationType.Low,
};

const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").delegatedPermissionClassifications.post(requestBody);
}


```