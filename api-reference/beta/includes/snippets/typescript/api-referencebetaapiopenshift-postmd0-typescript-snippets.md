---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const configuration = {
	headers : {
		"Authorization": "Bearer {token}",
	}
};
const requestBody : OpenShift = {
	id : "OPNSHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
	schedulingGroupId : "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
	sharedOpenShift : {
		notes : "InventoryManagement",
		openSlotCount : 2,
		displayName : "Dayshift",
		startDateTime : new Date("2018-10-04T00: 58: 45.340Z"),
		endDateTime : new Date("2018-10-04T09: 50: 45.332Z"),
		theme : ScheduleEntityTheme.White,
		activities : [
			{
				isPaid : true,
				startDateTime : new Date("2018-10-04T00: 58: 45.340Z"),
				endDateTime : new Date("2018-10-04T01: 58: 45.340Z"),
				code : "",
				displayName : "Lunch",
			},
		],
	},
	draftOpenShift : null,
	createdDateTime : new Date("2019-03-14T04: 32: 51.451Z"),
	lastModifiedDateTime : new Date("2019-03-14T05: 32: 51.451Z"),
	lastModifiedBy : {
		application : null,
		device : null,
		user : {
			id : "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
			displayName : "JohnDoe",
		},
		additionalData : {
			conversation : null,
		},
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.openShifts.post(requestBody, configuration);
}


```