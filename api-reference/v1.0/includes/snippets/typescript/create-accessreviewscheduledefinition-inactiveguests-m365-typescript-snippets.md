---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessReviewScheduleDefinition = {
	displayName : "Review inactive guests on teams",
	descriptionForAdmins : "Control guest user access to our teams.",
	descriptionForReviewers : "Information security is everyone's responsibility. Review our access policy for more.",
	instanceEnumerationScope : {
		"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
		additionalData : {
			"query" : "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
			"queryType" : "MicrosoftGraph",
		},
	},
	scope : {
		"@odata.type" : "#microsoft.graph.accessReviewInactiveUsersQueryScope",
		additionalData : {
			"query" : "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
			"queryType" : "MicrosoftGraph",
			"inactiveDuration" : "P30D",
		},
	},
	reviewers : [
		{
			query : "./owners",
			queryType : "MicrosoftGraph",
		},
	],
	fallbackReviewers : [
		{
			query : "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
			queryType : "MicrosoftGraph",
		},
	],
	settings : {
		mailNotificationsEnabled : true,
		reminderNotificationsEnabled : true,
		justificationRequiredOnApproval : true,
		recommendationsEnabled : true,
		instanceDurationInDays : 3,
		recurrence : {
			pattern : {
				type : RecurrencePatternType.AbsoluteMonthly,
				dayOfMonth : 5,
				interval : 3,
			},
			range : {
				type : RecurrenceRangeType.NoEnd,
				startDate : "2020-05-04T00:00:00.000Z",
			},
		},
		defaultDecisionEnabled : true,
		defaultDecision : "Deny",
		autoApplyDecisionsEnabled : true,
	},
};

const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitions.post(requestBody);
}


```