---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationalActivity = {
	institution : {
		location : {
			type : PhysicalAddressType.Business,
			postOfficeBox : null,
			street : "12000 E Prospect Rd",
			city : "Fort Collins",
			state : "Colorado",
			countryOrRegion : "USA",
			postalCode : "80525",
		},
	},
};

const result = async () => {
	await graphServiceClient.me.profile.educationalActivitiesById("educationalActivity-id").patch(requestBody);
}


```