---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Workflow = {
	category : LifecycleWorkflowCategory.Leaver,
	displayName : "Post-Offboarding of an employee",
	description : "Configure offboarding tasks for employees after their last day of work",
	isEnabled : true,
	isSchedulingEnabled : false,
	executionConditions : {
		"@odata.type" : "#microsoft.graph.identityGovernance.triggerAndScopeBasedConditions",
		additionalData : {
			scope : {
				"@odata.type" : "#microsoft.graph.identityGovernance.ruleBasedSubjectSet",
				rule : "department eq 'Marketing'",
			},
			trigger : {
				"@odata.type" : "#microsoft.graph.identityGovernance.timeBasedAttributeTrigger",
				timeBasedAttribute : "employeeLeaveDateTime",
				offsetInDays : 7,
			},
		},
	},
	tasks : [
		{
			category : LifecycleTaskCategory.Leaver,
			continueOnError : false,
			description : "Remove all licenses assigned to the user",
			displayName : "Remove all licenses for user",
			executionSequence : 1,
			isEnabled : true,
			taskDefinitionId : "8fa97d28-3e52-4985-b3a9-a1126f9b8b4e",
			arguments : [
			],
		},
		{
			category : LifecycleTaskCategory.Leaver,
			continueOnError : false,
			description : "Remove user from all Teams memberships",
			displayName : "Remove user from all Teams",
			executionSequence : 2,
			isEnabled : true,
			taskDefinitionId : "81f7b200-2816-4b3b-8c5d-dc556f07b024",
			arguments : [
			],
		},
		{
			category : LifecycleTaskCategory.Leaver,
			continueOnError : false,
			description : "Delete user account in Azure AD",
			displayName : "Delete User Account",
			executionSequence : 3,
			isEnabled : true,
			taskDefinitionId : "8d18588d-9ad3-4c0f-99d0-ec215f0e3dff",
			arguments : [
			],
		},
	],
};

const result = async () => {
	await graphServiceClient.identityGovernance.lifecycleWorkflows.workflows.post(requestBody);
}


```