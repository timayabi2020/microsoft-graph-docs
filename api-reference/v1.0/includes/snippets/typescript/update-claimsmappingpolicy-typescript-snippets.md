---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ClaimsMappingPolicy = {
	displayName : "UpdateClaimsPolicy",
};

const result = async () => {
	await graphServiceClient.policies.claimsMappingPoliciesById("claimsMappingPolicy-id").patch(requestBody);
}


```