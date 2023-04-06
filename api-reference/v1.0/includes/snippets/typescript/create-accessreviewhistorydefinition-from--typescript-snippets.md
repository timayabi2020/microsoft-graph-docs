---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : AccessReviewHistoryDefinition = {
	displayName : "Last quarter's group reviews April 2021",
	decisions : [
		accessReviewHistoryDecisionFilter : AccessReviewHistoryDecisionFilter.Approve,
		accessReviewHistoryDecisionFilter : AccessReviewHistoryDecisionFilter.Deny,
		accessReviewHistoryDecisionFilter : AccessReviewHistoryDecisionFilter.DontKnow,
		accessReviewHistoryDecisionFilter : AccessReviewHistoryDecisionFilter.NotReviewed,
		accessReviewHistoryDecisionFilter : AccessReviewHistoryDecisionFilter.NotNotified,
	],
	reviewHistoryPeriodStartDateTime : new Date("2021-01-01T00:00:00Z"),
	reviewHistoryPeriodEndDateTime : new Date("2021-04-30T23:59:59Z"),
	scopes : [
		{
			"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
			additionalData : {
				"queryType" : "MicrosoftGraph",
				"query" : "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'accessPackageAssignments')",
				queryRoot : null,
			},
		},
		{
			"@odata.type" : "#microsoft.graph.accessReviewQueryScope",
			additionalData : {
				"queryType" : "MicrosoftGraph",
				"query" : "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, '/groups')",
				queryRoot : null,
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.historyDefinitions.post(requestBody);
}


```