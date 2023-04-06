---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ConnectedOrganization = {
	displayName : "Connected organization new name",
	description : "Connected organization new description",
	state : ConnectedOrganizationState.Configured,
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.connectedOrganizationsById("connectedOrganization-id").patch(requestBody);
}


```