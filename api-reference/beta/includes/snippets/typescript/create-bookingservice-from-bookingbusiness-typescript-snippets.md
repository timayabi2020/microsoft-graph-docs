---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingService = {
	"@odata.type" : "#microsoft.graph.bookingService",
	defaultDuration : pT1H30M,
	defaultLocation : {
		"@odata.type" : "#microsoft.graph.location",
		address : {
			"@odata.type" : "#microsoft.graph.physicalAddress",
			city : "Buffalo",
			countryOrRegion : "USA",
			postalCode : "98052",
			postOfficeBox : null,
			state : "NY",
			street : "4567 First Street",
			type : null,
			additionalData : {
				"type@odata.type" : "#microsoft.graph.physicalAddressType",
			},
		},
		coordinates : null,
		displayName : "Contoso Lunch Delivery",
		locationEmailAddress : null,
		locationType : null,
		locationUri : null,
		uniqueId : null,
		uniqueIdType : null,
		additionalData : {
			"locationType@odata.type" : "#microsoft.graph.locationType",
			"uniqueIdType@odata.type" : "#microsoft.graph.locationUniqueIdType",
		},
	},
	defaultPrice : 10,
	defaultPriceType : BookingPriceType.FixedPrice,
	defaultReminders : [
		{
			"@odata.type" : "#microsoft.graph.bookingReminder",
			message : "Please be reminded that this service is tomorrow.",
			offset : p1D,
			recipients : BookingReminderRecipients.AllAttendees,
			additionalData : {
				"recipients@odata.type" : "#microsoft.graph.bookingReminderRecipients",
			},
		},
	],
	description : "Individual bento box lunch delivery",
	displayName : "Bento",
	isLocationOnline : true,
	smsNotificationsEnabled : true,
	languageTag : "en-US",
	isHiddenFromCustomers : false,
	notes : "Home-cooked special",
	postBuffer : pT10M,
	preBuffer : pT5M,
	schedulingPolicy : {
		"@odata.type" : "#microsoft.graph.bookingSchedulingPolicy",
		allowStaffSelection : true,
		maximumAdvance : p10D,
		minimumLeadTime : pT10H,
		sendConfirmationsToOwner : true,
		timeSlotInterval : pT1H,
	},
	staffMemberIds : [
		"d90d1e8c-5cfe-48cf-a2d5-966267375b6a",
		"2f5f8794-0b29-45b5-b56a-2eb5ff7aa880",
	],
	isAnonymousJoinEnabled : false,
	additionalData : {
		"defaultPriceType@odata.type" : "#microsoft.graph.bookingPriceType",
		"defaultReminders@odata.type" : "#Collection(microsoft.graph.bookingReminder)",
		"staffMemberIds@odata.type" : "#Collection(String)",
	},
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").services.post(requestBody);
}


```