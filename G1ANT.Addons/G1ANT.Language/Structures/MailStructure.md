# mail
Mail structure stores current information about a mail message, which was downloaded with the `mail.imap` command. The mail structure contains several fields such as:

| Field | Description | Type|
| -------- | ---- |------ |
|`id`| The identification number of the message. |string|
|`from`| The sender of the message. |string|
|`to`| The receiver of the message. |string|
|`subject`| The subject of the message. |string|
|`content`| The content of the message.|string|
|`dateIndex`| The date of the message.|date|
|`priorityIndex`| The priority of the message.|integer|
|`attachments`| The attachment names of the message.|int|
|`isReply`| Is the message a reply.|bool|

### Example
This example shows how to receive messages using the `mail.imap` command and iterate through all of them. As a result, the message body should be displayed in a dialog box.

```G1ANT

♥yesterday = ⟦date⟧13.01.2018
mail.imap host ‴imap.gmail.com‴ port ‴993‴ login ‴xx@gmail.com‴ password ‴yyyyyyy‴ sincedate ♥yesterday onlyunreadmessages true markallmessagesasread false result ♥result 

foreach ♥element in ♥result
   dialog ♥element⟦content⟧
end foreach

```
