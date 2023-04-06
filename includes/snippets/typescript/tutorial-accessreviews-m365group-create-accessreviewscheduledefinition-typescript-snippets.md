---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessReviewScheduleDefinition = {
	displayName : "Group owners review guest across Microsoft 365 groups in the tenant (Quarterly)",
	descriptionForAdmins : "",
	descriptionForReviewers : "",
	scope : {
		additionalData : {
			"query" : "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
			"queryType" : "MicrosoftGraph",
		},
	},
	instanceEnumerationScope : {
		additionalData : {
			"query" : "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
			"queryType" : "MicrosoftGraph",
		},
	},
	reviewers : [
		{
			query : "./owners",
			queryType : "MicrosoftGraph",
			queryRoot : null,
		},
	],
	fallbackReviewers : [
		{
			query : "/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4",
			queryType : "MicrosoftGraph",
			queryRoot : null,
		},
	],
	settings : {
		mailNotificationsEnabled : true,
		reminderNotificationsEnabled : true,
		justificationRequiredOnApproval : true,
		defaultDecisionEnabled : true,
		defaultDecision : "Approve",
		instanceDurationInDays : 0,
		autoApplyDecisionsEnabled : true,
		recommendationsEnabled : true,
		recurrence : {
			pattern : {
				type : RecurrencePatternType.AbsoluteMonthly,
				interval : 3,
				month : 0,
				dayOfMonth : 0,
				daysOfWeek : [
				],
				firstDayOfWeek : DayOfWeek.Sunday,
				index : WeekIndex.First,
			},
			range : {
				type : RecurrenceRangeType.Numbered,
				numberOfOccurrences : 0,
				recurrenceTimeZone : null,
				startDate : "2021-02-10",
				endDate : "2022-12-21",
			},
		},
		applyActions : [
			{
				"@odata.type" : "#microsoft.graph.removeAccessApplyAction",
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitions.post(requestBody);
}


```