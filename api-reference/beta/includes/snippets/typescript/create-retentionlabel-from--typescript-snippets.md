---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : RetentionLabel = {
	"@odata.type" : "#microsoft.graph.security.retentionLabel",
	displayName : "String",
	behaviorDuringRetentionPeriod : BehaviorDuringRetentionPeriod.String,
	actionAfterRetentionPeriod : ActionAfterRetentionPeriod.String,
	retentionTrigger : RetentionTrigger.String,
	retentionDuration : {
		"@odata.type" : "microsoft.graph.security.retentionDuration",
	},
	isInUse : boolean,
	descriptionForAdmins : "String",
	descriptionForUsers : "String",
	createdBy : {
		"@odata.type" : "microsoft.graph.identitySet",
	},
	labelToBeApplied : "String",
	defaultRecordBehavior : DefaultRecordBehavior.String,
};

const result = async () => {
	await graphServiceClient.security.labels.retentionLabels.post(requestBody);
}


```