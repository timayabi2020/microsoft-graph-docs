---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : WorkPosition = {
	detail : {
		company : {
			displayName : "Adventureworks Ltd.",
			department : "Consulting",
			officeLocation : "AW23/344",
			address : {
				type : PhysicalAddressType.Business,
				street : "123 Patriachy Ponds",
				city : "Moscow",
				countryOrRegion : "Russian Federation",
				postalCode : "RU-34621",
			},
			webUrl : "https://www.adventureworks.com",
		},
		jobTitle : "Senior Product Branding Manager II",
		role : "consulting",
	},
	isCurrent : true,
};

const result = async () => {
	await graphServiceClient.me.profile.positions.post(requestBody);
}


```