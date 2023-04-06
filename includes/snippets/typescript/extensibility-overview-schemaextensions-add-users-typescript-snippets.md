---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : User = {
	accountEnabled : true,
	displayName : "Adele Vance",
	mailNickname : "AdeleV",
	userPrincipalName : "AdeleV@m365x72712789.onmicrosoft.com",
	passwordProfile : {
		forceChangePasswordNextSignIn : false,
		password : "xWwvJ]6NMw+bWH-d",
	},
	additionalData : {
		extkmpdyld2_graphLearnCourses : {
			courseId : 100,
			courseName : "Explore Microsoft Graph",
			courseType : "Online",
		},
	},
};

const result = async () => {
	await graphServiceClient.users.post(requestBody);
}


```