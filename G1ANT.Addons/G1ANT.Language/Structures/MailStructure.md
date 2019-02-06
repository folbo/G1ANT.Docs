# mail
Mail structure stores current information about a mail message, which was downloaded with the `mail.imap` command. The mail structure contains several fields such as:

| Field | Type| Description |
| -------- |------ | ---- |
|`id`|text| The identification number of the message |
|`from`|text| The sender of the message |
|`to`|text| The recipient of the message |
|`subject`|text| The subject of the message |
|`content`|text| The content of the message |
|`dateIndex`|text| The date of the message |
|`priorityIndex`|integer| The priority of the message |
|`attachments`|list| Returns a list of elements of the [attachment](attachmentstructure.md) structure allowing to manage attachments |
|`isReply`|bool| Is the message a reply |

## Example
This example shows how to receive messages using the `mail.imap` command and iterate through all of them. As a result, the message body should be displayed in a dialog box.

```G1ANT
♥yesterday = ⟦date⟧13.01.2018
mail.imap host imap.gmail.com port 993 login mail@gmail.com password p@$$w0rD sincedate ♥yesterday onlyunreadmessages true markallmessagesasread false result ♥result 

foreach ♥element in ♥result
   dialog ♥element⟦content⟧
end foreach
```

> **Note:** Host, login and password values are of course just examples. You have to provide your real mail server credentials for the command to work.
