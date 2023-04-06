---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : BookingCustomerBase = {
	"@odata.type" : "#microsoft.graph.bookingCustomer",
	additionalData : {
		"displayName" : "Joni Sherman",
		"emailAddress" : "jonis@relecloud.com",
		addresses : [
			{
				postOfficeBox : "",
				street : "4567 Main Street",
				city : "Buffalo",
				state : "NY",
				countryOrRegion : "USA",
				postalCode : "98052",
				type : "home",
			},
			{
				postOfficeBox : "",
				street : "4570 Main Street",
				city : "Buffalo",
				state : "NY",
				countryOrRegion : "USA",
				postalCode : "98054",
				type : "business",
			},
		],
		phones : [
			{
				number : "206-555-0100",
				type : "home",
			},
			{
				number : "206-555-0200",
				type : "business",
			},
		],
	},
};

const result = async () => {
	await graphServiceClient.solutions.bookingBusinessesById("bookingBusiness-id").customers.post(requestBody);
}


```