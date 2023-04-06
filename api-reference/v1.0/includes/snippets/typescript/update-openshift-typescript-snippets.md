---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : OpenShift = {
	schedulingGroupId : "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
	sharedOpenShift : {
		notes : "Inventory Management",
		openSlotCount : 5,
		displayName : "Field shift",
		startDateTime : new Date("2018-10-04T00:58:45.340Z"),
		endDateTime : new Date("2018-10-04T09:50:45.332Z"),
		theme : ScheduleEntityTheme.White,
		activities : [
			{
				isPaid : true,
				startDateTime : new Date("2018-10-04T00:58:45.340Z"),
				endDateTime : new Date("2018-10-04T01:58:45.340Z"),
				code : "",
				displayName : "Lunch",
			},
		],
	},
	draftOpenShift : null,
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.openShiftsById("openShift-id").patch(requestBody);
}


```