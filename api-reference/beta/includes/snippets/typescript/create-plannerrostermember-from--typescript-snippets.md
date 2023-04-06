---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PlannerRosterMember = {
	"@odata.type" : "#microsoft.graph.plannerRosterMember",
	userId : "String",
};

const result = async () => {
	await graphServiceClient.planner.rostersById("plannerRoster-id").members.post(requestBody);
}


```