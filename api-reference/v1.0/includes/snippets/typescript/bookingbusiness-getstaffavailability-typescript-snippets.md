---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : GetStaffAvailabilityPostRequestBody = {
	staffIds : [
		"311a5454-08b2-4560-ba1c-f715e938cb79",
	],
	startDateTime : {
		dateTime : "2022-01-25T00:00:00",
		timeZone : "India Standard Time",
	},
	endDateTime : {
		dateTime : "2022-01-26T17:00:00",
		timeZone : "Pacific Standard Time",
	},
};

const result = async () => {
	await graphServiceClient.solutions.bookingBusinessesById("bookingBusiness-id").getStaffAvailability.post(requestBody);
}


```