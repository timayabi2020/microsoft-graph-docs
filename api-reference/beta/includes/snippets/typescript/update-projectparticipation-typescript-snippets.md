---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ProjectParticipation = {
	allowedAudiences : AllowedAudiences.Organization,
	client : {
		department : "Corporate Marketing",
		webUrl : "https://www.contoso.com",
	},
};

const result = async () => {
	await graphServiceClient.me.profile.projectsById("projectParticipation-id").patch(requestBody);
}


```