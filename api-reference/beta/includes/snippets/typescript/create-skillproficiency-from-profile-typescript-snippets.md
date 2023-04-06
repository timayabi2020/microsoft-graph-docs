---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : SkillProficiency = {
	categories : [
		"Professional",
	],
	allowedAudiences : AllowedAudiences.Organization,
	displayName : "API Design",
	proficiency : SkillProficiencyLevel.GeneralProfessional,
	collaborationTags : [
		"ableToMentor",
	],
};

const result = async () => {
	await graphServiceClient.me.profile.skills.post(requestBody);
}


```