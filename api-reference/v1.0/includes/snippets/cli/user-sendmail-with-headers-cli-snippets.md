---
description: "Automatically generated file. DO NOT MODIFY"
---

```cli

mgc me send-mail post --body '{\
  "message": {\
    "subject": "9/9/2018: concert",\
    "body": {\
      "contentType": "HTML",\
      "content": "The group represents Nevada."\
    },\
    "toRecipients": [\
      {\
        "emailAddress": {\
          "address": "AlexW@contoso.OnMicrosoft.com"\
        }\
      }\
    ],\
    "internetMessageHeaders":[\
      {\
        "name":"x-custom-header-group-name",\
        "value":"Nevada"\
      },\
      {\
        "name":"x-custom-header-group-id",\
        "value":"NV001"\
      }\
    ]\
  }\
}\
'

```