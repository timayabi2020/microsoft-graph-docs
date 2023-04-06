---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PlannerBucket = {
	name : "Advertising",
	planId : "xqQg5FS2LkCp935s-FIFm2QAFkHM",
	orderHint : " !",
};

const result = async () => {
	await graphServiceClient.planner.buckets.post(requestBody);
}


```