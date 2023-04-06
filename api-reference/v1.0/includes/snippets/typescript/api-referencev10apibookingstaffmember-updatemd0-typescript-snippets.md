---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingStaffMemberBase = {
	"@odata.type" : "#microsoft.graph.bookingStaffMember",
	additionalData : {
		workingHours : [
			{
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				day : "monday",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
				timeSlots : [
				],
			},
			{
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				day : "tuesday",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
				timeSlots : [
					{
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
						endTime : "17:00:00.0000000",
						startTime : "08:00:00.0000000",
					},
				],
			},
			{
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				day : "wednesday",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
				timeSlots : [
					{
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
						endTime : "17:00:00.0000000",
						startTime : "08:00:00.0000000",
					},
				],
			},
			{
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				day : "thursday",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
				timeSlots : [
					{
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
						endTime : "17:00:00.0000000",
						startTime : "08:00:00.0000000",
					},
				],
			},
			{
				"@odata.type" : "#microsoft.graph.bookingWorkHours",
				"day@odata.type" : "#microsoft.graph.dayOfWeek",
				day : "friday",
				"timeSlots@odata.type" : "#Collection(microsoft.graph.bookingWorkTimeSlot)",
				timeSlots : [
					{
						"@odata.type" : "#microsoft.graph.bookingWorkTimeSlot",
						endTime : "17:00:00.0000000",
						startTime : "08:00:00.0000000",
					},
				],
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.solutions.bookingBusinessesById("bookingBusiness-id").staffMembersById("bookingStaffMemberBase-id").patch(requestBody);
}


```