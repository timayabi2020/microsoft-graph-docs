---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingStaffMember = {
	workingHours : [
		{
			"@odata.type" : "#microsoft.graph.bookingWorkHours",
			day : DayOfWeek.Monday,
			timeSlots : [
			],
			additionalData : {
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.bookingWorkHours",
			day : DayOfWeek.Tuesday,
			timeSlots : [
				{
					"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					end : 17:00:00.0000000,
					start : 08:00:00.0000000,
				},
			],
			additionalData : {
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.bookingWorkHours",
			day : DayOfWeek.Wednesday,
			timeSlots : [
				{
					"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					end : 17:00:00.0000000,
					start : 08:00:00.0000000,
				},
			],
			additionalData : {
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.bookingWorkHours",
			day : DayOfWeek.Thursday,
			timeSlots : [
				{
					"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					end : 17:00:00.0000000,
					start : 08:00:00.0000000,
				},
			],
			additionalData : {
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.bookingWorkHours",
			day : DayOfWeek.Friday,
			timeSlots : [
				{
					"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
					end : 17:00:00.0000000,
					start : 08:00:00.0000000,
				},
			],
			additionalData : {
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
			},
		},
	],
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").staffMembersById("bookingStaffMember-id").patch(requestBody);
}


```