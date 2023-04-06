---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ProjectParticipation = {
	categories : [
		"Branding",
	],
	client : {
		displayName : "Contoso Ltd.",
		department : "Corporate Marketing",
		webUrl : "https://www.contoso.com",
	},
	displayName : "Contoso Re-branding Project",
	detail : {
		company : {
			displayName : "Adventureworks Inc.",
			department : "Consulting",
			webUrl : "https://adventureworks.com",
		},
		description : "Rebranding of Contoso Ltd.",
		jobTitle : "Lead PM Rebranding",
		role : "project management",
		summary : "A 6 month project to help Contoso rebrand after they were divested from a parent organization.",
	},
};

const result = async () => {
	await graphServiceClient.me.profile.projects.post(requestBody);
}


```