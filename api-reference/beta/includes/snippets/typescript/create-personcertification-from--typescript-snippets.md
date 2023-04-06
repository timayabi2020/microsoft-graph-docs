---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PersonCertification = {
	certificationId : "KB-1235466333663322",
	description : "Blackbelt in Marketing - Brand Management",
	displayName : "Marketing Blackbelt - Brand Management",
	thumbnailUrl : "https://iame.io/dfhdfdfd334.jpg",
	webUrl : "https://www.iame.io/blackbelt",
};

const result = async () => {
	await graphServiceClient.me.profile.certifications.post(requestBody);
}


```