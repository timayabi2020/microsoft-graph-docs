---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"ConsistencyLevel": "eventual",
	}
,	queryParameters : {
		filter: "mailEnabled eq false and securityEnabled eq true and NOT) and membershipRuleProcessingState eq 'On'",
		count: true,
		select: ["id","membershipRule","membershipRuleProcessingState"],
	}
};

const result = async () => {
	await graphServiceClient.groups.get(configuration);
}


```