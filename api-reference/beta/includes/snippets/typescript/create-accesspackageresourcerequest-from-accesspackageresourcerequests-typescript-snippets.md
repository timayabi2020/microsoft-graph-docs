---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageResourceRequest = {
	catalogId : "26ac0c0a-08bc-4a7b-a313-839f58044ba5",
	requestType : "AdminAdd",
	justification : "",
	accessPackageResource : {
		displayName : "Sales",
		description : "https://contoso.sharepoint.com/sites/Sales",
		url : "https://contoso.sharepoint.com/sites/Sales",
		resourceType : "SharePoint Online Site",
		originId : "https://contoso.sharepoint.com/sites/Sales",
		originSystem : "SharePointOnline",
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(requestBody);
}


```