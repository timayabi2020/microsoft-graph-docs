---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessReviewScheduleDefinition = {
	displayName : "Group Multi-stage Access Review",
	descriptionForAdmins : "New scheduled access review",
	descriptionForReviewers : "If you have any questions, contact jerry@contoso.com",
	scope : {
		"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
		additionalData : {
			"query" : "/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers",
			"queryType" : "MicrosoftGraph",
		},
	},
	stageSettings : [
		{
			stageId : "1",
			durationInDays : 2,
			recommendationsEnabled : false,
			decisionsThatWillMoveToNextStage : [
				"NotReviewed",
				"Approve",
			],
			reviewers : [
				{
					query : "/users/398164b1-5196-49dd-ada2-364b49f99b27",
					queryType : "MicrosoftGraph",
				},
			],
		},
		{
			stageId : "2",
			dependsOn : [
				"1",
			],
			durationInDays : 2,
			recommendationsEnabled : true,
			reviewers : [
				{
					query : "./manager",
					queryType : "MicrosoftGraph",
					queryRoot : "decisions",
				},
			],
			fallbackReviewers : [
				{
					query : "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
					queryType : "MicrosoftGraph",
				},
			],
		},
	],
	settings : {
		mailNotificationsEnabled : true,
		reminderNotificationsEnabled : true,
		justificationRequiredOnApproval : true,
		defaultDecisionEnabled : false,
		defaultDecision : "None",
		instanceDurationInDays : 4,
		recurrence : {
			pattern : {
				type : RecurrencePatternType.Weekly,
				interval : 1,
			},
			range : {
				type : RecurrenceRangeType.NoEnd,
				startDate : "2020-09-08T12:02:30.667Z",
			},
		},
		decisionHistoriesForReviewersEnabled : true,
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitions.post(requestBody);
}


```