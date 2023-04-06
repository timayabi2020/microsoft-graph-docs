---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TimeCard = {
	additionalData : {
		"userId" : "70e47528-2fae-42b5-9d8e-ee73ccd90603",
		"state" : "clockedOut",
		"confirmedBy" : "None",
		notes : null,
		clockInEvent : {
			dateTime : "2021-05-21T21:58:41.327Z",
			atApprovedLocation : null,
			notes : {
				contentType : "text",
				content : "update sample notes",
			},
		},
		clockOutEvent : {
			dateTime : "2021-05-21T22:01:46.205Z",
			atApprovedLocation : null,
			notes : {
				contentType : "text",
				content : "update sample notes",
			},
		},
		breaks : [
			{
				breakId : "BRK_138f4751-68b1-44c1-aca2-2b26cba9e73f",
				notes : null,
				start : {
					dateTime : "2021-05-21T21:59:59.328Z",
					atApprovedLocation : null,
					notes : {
						contentType : "text",
						content : "update sample notes",
					},
				},
				end : {
					dateTime : "2021-05-21T22:01:10.205Z",
					atApprovedLocation : null,
					notes : {
						contentType : "text",
						content : "update sample notes",
					},
				},
			},
		],
	},
};

async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeCardsById("timeCard-id").put(requestBody);
}


```