---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : TimeCard = {
	clockInEvent : {
		dateTime : new Date("2019-03-18T00:00:00.000Z"),
		atApprovedLocation : true,
		notes : {
			content : "Started late due to traffic in CA 237",
			contentType : BodyType.Text,
		},
	},
	notes : {
		content : "8 To 5 Inventory management",
		contentType : BodyType.Text,
	},
	breaks : [
		{
			breakId : "string",
			notes : {
				content : "Lunch break",
				contentType : BodyType.Text,
			},
			start : {
				dateTime : new Date("2019-03-18T02:00:00.000Z"),
				atApprovedLocation : true,
				notes : {
					content : "Reduced break to make up for lost time",
					contentType : BodyType.Text,
				},
			},
		},
	],
	additionalData : {
		"onBehalfOfUserId" : "a3601044-a1b5-438e-b742-f78d01d68a67",
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeCards.post(requestBody);
}


```