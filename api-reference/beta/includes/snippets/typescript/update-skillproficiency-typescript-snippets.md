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
	proficiency : SkillProficiencyLevel.AdvancedProfessional,
};

const result = async () => {
	await graphServiceClient.me.profile.skillsById("skillProficiency-id").patch(requestBody);
}


```