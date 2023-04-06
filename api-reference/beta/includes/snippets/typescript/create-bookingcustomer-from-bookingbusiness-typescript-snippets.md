---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingCustomer = {
	displayName : "Joni Sherman",
	emailAddress : "jonis@relecloud.com",
	addresses : [
		{
			postOfficeBox : "",
			street : "4567 Main Street",
			city : "Buffalo",
			state : "NY",
			countryOrRegion : "USA",
			postalCode : "98052",
			type : PhysicalAddressType.Home,
		},
		{
			postOfficeBox : "",
			street : "4570 Main Street",
			city : "Buffalo",
			state : "NY",
			countryOrRegion : "USA",
			postalCode : "98054",
			type : PhysicalAddressType.Business,
		},
	],
	phones : [
		{
			number : "206-555-0100",
			type : PhoneType.Home,
		},
		{
			number : "206-555-0200",
			type : PhoneType.Business,
		},
	],
};

const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").customers.post(requestBody);
}


```