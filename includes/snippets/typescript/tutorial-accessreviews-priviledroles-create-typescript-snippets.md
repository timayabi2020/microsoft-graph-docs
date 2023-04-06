---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessReviewScheduleDefinition = {
	displayName : "Review access of users and groups to privileged roles",
	descriptionForAdmins : "Review access of users and groups to privileged roles",
	scope : {
		"@odata.type" : "#microsoft.graph.principalResourceMembershipsScope",
		additionalData : {
			principalScopes : [
				{
					"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
					query : "/users",
					queryType : "MicrosoftGraph",
				},
				{
					"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
					query : "/groups",
					queryType : "MicrosoftGraph",
				},
			],
			resourceScopes : [
				{
					"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
					query : "/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
					queryType : "MicrosoftGraph",
				},
			],
		},
	},
	reviewers : [
		{
			query : "/users/f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
			queryType : "MicrosoftGraph",
		},
	],
	settings : {
		mailNotificationsEnabled : true,
		reminderNotificationsEnabled : true,
		justificationRequiredOnApproval : true,
		defaultDecisionEnabled : false,
		defaultDecision : "None",
		instanceDurationInDays : 3,
		recommendationsEnabled : false,
		recurrence : {
			pattern : {
				type : RecurrencePatternType.AbsoluteMonthly,
				interval : 3,
			},
			range : {
				type : RecurrenceRangeType.NoEnd,
				startDate : "2022-03-02",
			},
		},
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitions.post(requestBody);
}


```