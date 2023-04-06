---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ShiftPreferences = {
	id : "SHPR_eeab4fb1-20e5-48ca-ad9b-98119d94bee7",
	availability : [
		{
			recurrence : {
				pattern : {
					type : RecurrencePatternType.Weekly,
					daysOfWeek : [
						dayOfWeek : DayOfWeek.Monday,
						dayOfWeek : DayOfWeek.Wednesday,
						dayOfWeek : DayOfWeek.Friday,
					],
					interval : 1,
				},
				range : {
					type : RecurrenceRangeType.NoEnd,
				},
			},
			timeZone : "Pacific Standard Time",
			timeSlots : null,
		},
	],
	additionalData : {
		"@odata.etag" : "1a371e53-f0a6-4327-a1ee-e3c56e4b38aa",
	},
};

const result = async () => {
	await graphServiceClient.usersById("user-id").settings.shiftPreferences.patch(requestBody);
}


```