---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PersonAward = {
	description : "Lifetime Achievement award from the International Association of Branding Managers",
	displayName : "Lifetime Achievement Award For Excellence in Branding",
	issuedDate : "Date",
	issuingAuthority : "International Association of Branding Management",
	thumbnailUrl : "https://iabm.io/sdhdfhsdhshsd.jpg",
	webUrl : "https://www.iabm.io",
};

const result = async () => {
	await graphServiceClient.me.profile.awards.post(requestBody);
}


```