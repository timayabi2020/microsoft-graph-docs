---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	queryParameters : {
		expand: ["requestor($expand=connectedOrganization)"],
		filter: "(requestState eq 'PendingApproval')",
	}
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageAssignmentRequests.get(configuration);
}


```