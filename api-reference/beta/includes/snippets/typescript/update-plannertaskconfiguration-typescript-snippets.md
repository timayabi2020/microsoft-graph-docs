---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PlannerTaskConfiguration = {
	"@odata.type" : "#microsoft.graph.plannerTaskConfiguration",
	editPolicy : {
		rules : [
			{
				defaultRule : "block",
				role : {
					"@odata.type" : "#microsoft.graph.plannerRelationshipBasedUserType",
					roleKind : PlannerUserRoleKind.Relationship,
					additionalData : {
						"role" : "defaultRules",
					},
				},
				propertyRule : {
					percentComplete : [
						"allow",
					],
					ruleKind : PlannerRuleKind.TaskRule,
					assignments : {
						defaultRules : [
							"addSelf",
						],
						overrides : [
						],
					},
				},
			},
			{
				defaultRule : "block",
				role : {
					"@odata.type" : "#microsoft.graph.plannerRelationshipBasedUserType",
					roleKind : PlannerUserRoleKind.Relationship,
					additionalData : {
						"role" : "taskAssignees",
					},
				},
				propertyRule : {
					startDate : [
						"allow",
					],
					dueDate : [
						"allow",
					],
					percentComplete : [
						"allow",
					],
					order : [
						"allow",
					],
					ruleKind : PlannerRuleKind.TaskRule,
					references : {
						defaultRules : [
							"allow",
						],
						overrides : [
							{
								name : "userCreated",
								rules : [
									"allow",
								],
							},
							{
								name : "applicationCreated",
								rules : [
									"block",
								],
							},
						],
					},
					checkLists : {
						defaultRules : [
							"allow",
						],
						overrides : [
							{
								name : "userCreated",
								rules : [
									"allow",
								],
							},
							{
								name : "applicationCreated",
								rules : [
									"check",
								],
							},
						],
					},
					assignments : {
						defaultRules : [
							"block",
						],
						overrides : [
							{
								name : "userCreated",
								rules : [
									"removeSelf",
								],
							},
							{
								name : "applicationCreated",
								rules : [
									"check",
								],
							},
						],
					},
					appliedCategories : {
						defaultRules : [
							"allow",
						],
						overrides : [
						],
					},
				},
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.solutions.businessScenariosById("businessScenario-id").planner.taskConfiguration.patch(requestBody);
}


```