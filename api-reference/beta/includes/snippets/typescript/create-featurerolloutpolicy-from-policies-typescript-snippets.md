---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : FeatureRolloutPolicy = {
	displayName : "PassthroughAuthentication rollout policy",
	description : "PassthroughAuthentication rollout policy",
	feature : StagedFeatureName.PassthroughAuthentication,
	isEnabled : true,
	isAppliedToOrganization : false,
};

const result = async () => {
	await graphServiceClient.policies.featureRolloutPolicies.post(requestBody);
}


```