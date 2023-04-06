---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationClass = {
	description : "Health Level 1",
	classCode : "Health 501",
	displayName : "Health 1",
	externalId : "11019",
	externalName : "Health Level 1",
	externalSource : EducationExternalSource.Sis,
	mailNickname : "fineartschool.net",
};

const result = async () => {
	await graphServiceClient.education.classes.post(requestBody);
}


```