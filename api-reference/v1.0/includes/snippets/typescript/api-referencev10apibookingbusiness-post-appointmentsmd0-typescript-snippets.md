---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingAppointment = {
	"@odata.type" : "#microsoft.graph.bookingAppointment",
	customerTimeZone : "America/Chicago",
	smsNotificationsEnabled : true,
	endDateTime : {
		"@odata.type" : "#microsoft.graph.dateTimeTimeZone",
		dateTime : "2018-05-01T12:30:00.0000000+00:00",
		timeZone : "UTC",
	},
	isLocationOnline : true,
	optOutOfCustomerEmail : false,
	anonymousJoinWebUrl : null,
	postBuffer : pT10M,
	preBuffer : pT5M,
	price : 10,
	priceType : BookingPriceType.FixedPrice,
	reminders : [
		{
			"@odata.type" : "#microsoft.graph.bookingReminder",
			message : "This service is tomorrow",
			offset : p1D,
			recipients : BookingReminderRecipients.AllAttendees,
			additionalData : {
				"recipients@odata.type" : "#microsoft.graph.bookingReminderRecipients",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.bookingReminder",
			message : "Please be available to enjoy your lunch service.",
			offset : pT1H,
			recipients : BookingReminderRecipients.Customer,
			additionalData : {
				"recipients@odata.type" : "#microsoft.graph.bookingReminderRecipients",
			},
		},
		{
			"@odata.type" : "#microsoft.graph.bookingReminder",
			message : "Please check traffic for next cater.",
			offset : pT2H,
			recipients : BookingReminderRecipients.Staff,
			additionalData : {
				"recipients@odata.type" : "#microsoft.graph.bookingReminderRecipients",
			},
		},
	],
	serviceId : "57da6774-a087-4d69-b0e6-6fb82c339976",
	serviceLocation : {
		"@odata.type" : "#microsoft.graph.location",
		address : {
			"@odata.type" : "#microsoft.graph.physicalAddress",
			city : "Buffalo",
			countryOrRegion : "USA",
			postalCode : "98052",
			state : "NY",
			street : "123 First Avenue",
			additionalData : {
				postOfficeBox : null,
				"type@odata.type" : "#microsoft.graph.physicalAddressType",
				type : null,
			},
		},
		coordinates : null,
		displayName : "Customer location",
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
	serviceName : "Catered bento",
	serviceNotes : "Customer requires punctual service.",
	startDateTime : {
		"@odata.type" : "#microsoft.graph.dateTimeTimeZone",
		dateTime : "2018-05-01T12:00:00.0000000+00:00",
		timeZone : "UTC",
	},
	maximumAttendeesCount : 5,
	filledAttendeesCount : 1,
	customers : [
		{
			"@odata.type" : "#microsoft.graph.bookingCustomerInformation",
			additionalData : {
				"customerId" : "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
				"name" : "Jordan Miller",
				"emailAddress" : "jordanm@contoso.com",
				"phone" : "213-555-0199",
				notes : null,
				location : {
					"@odata.type" : "#microsoft.graph.location",
					displayName : "Customer",
					locationEmailAddress : null,
					locationUri : "",
					locationType : null,
					uniqueId : null,
					uniqueIdType : null,
					address : {
						"@odata.type" : "#microsoft.graph.physicalAddress",
						street : "",
						city : "",
						state : "",
						countryOrRegion : "",
						postalCode : "",
					},
					coordinates : {
						altitude : null,
						latitude : null,
						longitude : null,
						accuracy : null,
						altitudeAccuracy : null,
					},
				},
				"timeZone" : "America/Chicago",
				customQuestionAnswers : [
					{
						questionId : "3bc6fde0-4ad3-445d-ab17-0fc15dba0774",
						question : "What is your age?",
						answerInputType : "text",
						answerOptions : [
						],
						isRequired : true,
						answer : "25",
						selectedOptions : [
						],
					},
				],
			},
		},
	],
	additionalData : {
		"priceType@odata.type" : "#microsoft.graph.bookingPriceType",
		"reminders@odata.type" : "#Collection(microsoft.graph.bookingReminder)",
		"customers@odata.type" : "#Collection(microsoft.graph.bookingCustomerInformation)",
	},
};

const result = async () => {
	await graphServiceClient.solutions.bookingBusinessesById("bookingBusiness-id").appointments.post(requestBody);
}


```