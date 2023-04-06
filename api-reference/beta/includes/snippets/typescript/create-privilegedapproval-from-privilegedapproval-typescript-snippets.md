---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : PrivilegedApproval = {
	userId : "userId-value",
	roleId : "roleId-value",
	approvalType : "approvalType-value",
	approvalState : ApprovalState.ApprovalState-value,
	approvalDuration : datetime-value,
};

const result = async () => {
	await graphServiceClient.privilegedApproval.post(requestBody);
}


```