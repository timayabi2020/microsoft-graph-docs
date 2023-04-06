---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SubjectRightsRequest = {
	type : SubjectRightsRequestType.Export,
	contentQuery : "((\"Diego Siciliani\" OR \"Diego.Siciliani@contoso.com\") OR (participants:\"Diego.Siciliani@contoso.com\"))",
	dataSubjectType : DataSubjectType.Customer,
	externalId : "F53BF2DA-607D-412A-B568-FAA0F023AC0B",
	displayName : "Export report for customer Id: 12345",
	description : "This is a export request",
	includeAllVersions : false,
	includeAuthoredContent : true,
	internalDueDateTime : new Date("2022-07-20T22:42:28Z"),
	dataSubject : {
		firstName : "Diego",
		lastName : "Siciliani",
		email : "Diego.Siciliani@contoso.com",
		residency : "USA",
	},
	mailboxLocations : null,
	pauseAfterEstimate : true,
	regulations : [
		"CCPA",
	],
	siteLocations : {
		"@odata.type" : "microsoft.graph.subjectRightsRequestAllSiteLocation",
	},
};

const result = async () => {
	await graphServiceClient.privacy.subjectRightsRequests.post(requestBody);
}


```