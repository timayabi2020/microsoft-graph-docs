---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ConnectedOrganization = {
	displayName : "Connected organization name",
	description : "Connected organization description",
	identitySources : [
		{
			"@odata.type" : "#microsoft.graph.domainIdentitySource",
			additionalData : {
				"domainName" : "example.com",
				"displayName" : "example.com",
			},
		},
	],
	state : ConnectedOrganizationState.Proposed,
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.connectedOrganizations.post(requestBody);
}


```