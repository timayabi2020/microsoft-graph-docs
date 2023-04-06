---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PersonCertification = {
	issuingAuthority : "International Academy of Marketing Excellence",
	issuingCompany : "International Academy of Marketing Excellence",
};

const result = async () => {
	await graphServiceClient.usersById("user-id").profile.certificationsById("personCertification-id").patch(requestBody);
}


```