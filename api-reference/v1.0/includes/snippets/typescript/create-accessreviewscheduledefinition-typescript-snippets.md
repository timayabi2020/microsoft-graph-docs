---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessReviewScheduleDefinition = {
	displayName : "Test create",
	descriptionForAdmins : "New scheduled access review",
	descriptionForReviewers : "If you have any questions, contact jerry@contoso.com",
	scope : {
		"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
		additionalData : {
			"query" : "/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers",
			"queryType" : "MicrosoftGraph",
		},
	},
	reviewers : [
		{
			query : "/users/398164b1-5196-49dd-ada2-364b49f99b27",
			queryType : "MicrosoftGraph",
		},
	],
	settings : {
		mailNotificationsEnabled : true,
		reminderNotificationsEnabled : true,
		justificationRequiredOnApproval : true,
		defaultDecisionEnabled : false,
		defaultDecision : "None",
		instanceDurationInDays : 1,
		recommendationsEnabled : true,
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
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitions.post(requestBody);
}


```