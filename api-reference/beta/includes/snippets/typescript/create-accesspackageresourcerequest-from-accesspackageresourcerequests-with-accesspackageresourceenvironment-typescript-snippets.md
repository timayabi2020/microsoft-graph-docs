---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessPackageResourceRequest = {
	catalogId : "de9315c1-272b-4905-924b-cc112ca180c7",
	accessPackageResource : {
		displayName : "Community Outreach",
		description : "https://contoso.sharepoint.com/sites/CSR",
		resourceType : "SharePoint Online Site",
		originId : "https://contoso.sharepoint.com/sites/CSR",
		originSystem : "SharePointOnline",
		additionalData : {
			"accessPackageResourceEnvironment@odata.bind" : "accessPackageResourceEnvironments/615f2218-678f-471f-a60a-02c2f4f80c57",
		},
	},
	requestType : "AdminAdd",
};

const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageResourceRequests.post(requestBody);
}


```