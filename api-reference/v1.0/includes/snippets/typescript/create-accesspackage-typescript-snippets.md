---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackage = {
	displayName : "sales reps",
	description : "outside sales representatives",
	isHidden : false,
	catalog : {
		id : "66584aae-98bb-48cc-9458-7bee5d2a6577",
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackages.post(requestBody);
}


```