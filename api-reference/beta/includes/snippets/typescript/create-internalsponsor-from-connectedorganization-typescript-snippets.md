---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ReferenceCreate = {
	"@odata.id" : "https://graph.microsoft.com/beta/users/{id}",
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.connectedOrganizationsById("connectedOrganization-id").internalSponsors.$ref.post(requestBody);
}


```