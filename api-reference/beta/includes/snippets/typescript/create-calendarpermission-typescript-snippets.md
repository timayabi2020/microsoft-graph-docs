---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : CalendarPermission = {
	emailAddress : {
		name : "Samantha Booth",
		address : "samanthab@adatum.onmicrosoft.com",
	},
	isInsideOrganization : true,
	isRemovable : true,
	role : CalendarRoleType.Read,
};

const result = async () => {
	await graphServiceClient.usersById("user-id").calendar.calendarPermissions.post(requestBody);
}


```