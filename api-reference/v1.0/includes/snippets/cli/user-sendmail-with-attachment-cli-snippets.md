---
description: "Automatically generated file. DO NOT MODIFY"
---

```cli

mgc me send-mail post --body '{\
  "message": {\
    "subject": "Meet for lunch?",\
    "body": {\
      "contentType": "Text",\
      "content": "The new cafeteria is open."\
    },\
    "toRecipients": [\
      {\
        "emailAddress": {\
          "address": "meganb@contoso.onmicrosoft.com"\
        }\
      }\
    ],\
    "attachments": [\
      {\
        "@odata.type": "#microsoft.graph.fileAttachment",\
        "name": "attachment.txt",\
        "contentType": "text/plain",\
        "contentBytes": "SGVsbG8gV29ybGQh"\
      }\
    ]\
  }\
}\
'

```