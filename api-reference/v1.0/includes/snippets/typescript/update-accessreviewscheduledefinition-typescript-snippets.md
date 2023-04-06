---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : Definition = {
	additionalData : {
		"id" : "60860cdd-fb4d-4054-91ba-f75e04444aa6",
		"displayName" : "Test world UPDATED NAME!",
		"descriptionForAdmins" : "Test world",
		"descriptionForReviewers" : "Test world",
		scope : {
			"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
			query : "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
			queryType : "MicrosoftGraph",
		},
		instanceEnumerationScope : {
			"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
			query : "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f",
			queryType : "MicrosoftGraph",
		},
		reviewers : [
		],
		settings : {
			mailNotificationsEnabled : true,
			reminderNotificationsEnabled : true,
			justificationRequiredOnApproval : true,
			defaultDecisionEnabled : false,
			defaultDecision : "None",
			instanceDurationInDays : 3,
			autoApplyDecisionsEnabled : false,
			recommendationsEnabled : true,
			recurrence : {
				pattern : {
					type : "weekly",
					interval : 1,
				},
				range : {
					type : "noEnd",
					startDate : "2020-09-15",
				},
			},
		},
	},
};

async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitionsById("accessReviewScheduleDefinition-id").put(requestBody);
}


```