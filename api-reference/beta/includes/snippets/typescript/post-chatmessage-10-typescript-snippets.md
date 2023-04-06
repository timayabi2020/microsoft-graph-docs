---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody : ChatMessage = {
	subject : null,
	body : {
		contentType : BodyType.Html,
		content : "<attachment id=\"74d20c7f34aa4a7fb74e2b30004247c5\"></attachment>",
	},
	attachments : [
		{
			id : "74d20c7f34aa4a7fb74e2b30004247c5",
			contentType : "application/vnd.microsoft.card.thumbnail",
			contentUrl : null,
			content : "{\r\n  \"title\": \"This is an example of posting a card\",\r\n  \"subtitle\": \"<h3>This is the subtitle</h3>\",\r\n  \"text\": \"Here is some body text. <br>\r\nAnd a <a href=\\"http://microsoft.com/\\">hyperlink</a>. <br>\r\nAnd below that is some buttons:\",\r\n  \"buttons\": [\r\n    {\r\n      \"type\": \"messageBack\",\r\n      \"title\": \"Login to FakeBot\",\r\n      \"text\": \"login\",\r\n      \"displayText\": \"login\",\r\n      \"value\": \"login\"\r\n    }\r\n  ]\r\n}",
			name : null,
			thumbnailUrl : null,
			teamsAppId : "881b8843-fd91-49e5-9ac2-47ec497ffbe5",
		},
	],
};

const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.post(requestBody);
}


```