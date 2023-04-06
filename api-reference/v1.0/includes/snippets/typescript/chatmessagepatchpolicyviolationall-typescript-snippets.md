---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChatMessage = {
	policyViolation : {
		policyTip : {
			generalText : "This item has been blocked by the administrator.",
			complianceUrl : "https://contoso.com/dlp-policy-page",
			matchedConditionDescriptions : [
				"Credit Card Number",
			],
		},
		verdictDetails : ChatMessagePolicyViolationVerdictDetailsTypes.AllowOverrideWithoutJustification,AllowFalsePositiveOverride,
		dlpAction : ChatMessagePolicyViolationDlpActionTypes.BlockAccess,
	},
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messagesById("chatMessage-id").patch(requestBody);
}


```