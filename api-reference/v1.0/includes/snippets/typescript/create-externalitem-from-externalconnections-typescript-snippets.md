---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ExternalItem = {
	acl : [
		{
			type : AclType.User,
			value : "e811976d-83df-4cbd-8b9b-5215b18aa874",
			accessType : AccessType.Grant,
		},
		{
			type : AclType.ExternalGroup,
			value : "14m1b9c38qe647f6a",
			accessType : AccessType.Deny,
		},
	],
	properties : {
		additionalData : {
			"title" : "Error in the payment gateway",
			priority : 1,
			"assignee" : "john@contoso.com",
		},
	},
	content : {
		value : "Error in payment gateway...",
		type : ExternalItemContentType.Text,
	},
};

const result = async () => {
	await graphServiceClient.external.connectionsById("externalConnection-id").itemsById("externalItem-id").put(requestBody);
}


```