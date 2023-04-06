---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : EducationUser = {
	relatedContacts : [
		{
			displayName : "Father Time",
			emailAddress : "father@time.com",
			mobilePhone : "4251231234",
			relationship : ContactRelationship.Guardian,
			accessConsent : true,
		},
		{
			displayName : "Mother Nature",
			emailAddress : "mother@nature.co.uk",
			mobilePhone : "3251231234",
			relationship : ContactRelationship.Parent,
			accessConsent : true,
		},
	],
};

const result = async () => {
	await graphServiceClient.education.usersById("educationUser-id").patch(requestBody);
}


```