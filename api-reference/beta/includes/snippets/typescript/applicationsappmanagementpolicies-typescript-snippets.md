---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ReferenceCreate = {
	"@odata.id" : "https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}",
};

const result = async () => {
	await graphServiceClient.applicationsById("application-id").appManagementPolicies.$ref.post(requestBody);
}


```