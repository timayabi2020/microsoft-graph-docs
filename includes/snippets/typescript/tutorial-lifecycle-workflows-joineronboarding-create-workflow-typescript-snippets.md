---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Workflow = {
	displayName : "Onboard pre-hire employee",
	description : "Configure pre-hire tasks for onboarding employees before their first day",
	isEnabled : true,
	isSchedulingEnabled : false,
	executionConditions : {
		"@odata.type" : "microsoft.graph.identityGovernance.triggerAndScopeBasedConditions",
		additionalData : {
			scope : {
				"@odata.type" : "microsoft.graph.identityGovernance.ruleBasedSubjectSet",
				rule : "(department eq 'Sales')",
			},
			trigger : {
				"@odata.type" : "microsoft.graph.identityGovernance.timeBasedAttributeTrigger",
				timeBasedAttribute : "employeeHireDate",
				offsetInDays : -2,
			},
		},
	},
	tasks : [
		{
			isEnabled : true,
			category : LifecycleTaskCategory.Joiner,
			taskDefinitionId : "1b555e50-7f65-41d5-b514-5894a026d10d",
			displayName : "Generate TAP And Send Email",
			description : "Generate Temporary Access Pass and send via email to user's manager",
			arguments : [
				{
					name : "tapLifetimeMinutes",
					value : "480",
				},
				{
					name : "tapIsUsableOnce",
					value : "true",
				},
			],
		},
	],
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.workflows.post(requestBody);
}


```