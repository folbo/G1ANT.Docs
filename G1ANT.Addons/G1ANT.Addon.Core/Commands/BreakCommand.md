# break

**Syntax:**

```G1ANT
break
```

**Description:**

The break command immediately exits current block and continues process execution.

| Argument | Type | Required | Default Value | Description |
| -------- | ---- | -------- | ------------- | ----------- |
| if | bool | no | true | runs the command only if condition is true |
| timeout | [variable](https://github.com/G1ANT-Robot/G1ANT.Manual/blob/master/G1ANT-Language/Special-Characters/variable.md) | no | [♥timeoutcommand](https://github.com/G1ANT-Robot/G1ANT.Manual/blob/master/G1ANT-Language/Variables/Special-Variables.md) | specifies time in milliseconds for G1ANT.Robot to wait for the command to be executed |
| errorjump | [label](https://github.com/G1ANT-Robot/G1ANT.Manual/blob/master/G1ANT-Language/Structures/label.md) | no | | name of the label to jump to if a command throws an exception |
| errorcall | [procedure](https://github.com/G1ANT-Robot/G1ANT.Manual/blob/master/G1ANT-Language/Structures/procedure.md) | no | | name of the procedure to call if a command throws an exception |
| errorresult | [error](https://github.com/G1ANT-Robot/G1ANT.Manual/blob/master/G1ANT-Language/Structures/error.md) | no | | name of a variable, which will store the returned exception |
| errormessage | [text](https://github.com/G1ANT-Robot/G1ANT.Manual/blob/master/G1ANT-Language/Structures/text.md) | no | | message that will be shown in case error occurs and no errorjump argument is specified |

For more information about `if`, `timeout`, `errorjump`, `errorcall`, `errorresult` and `errormessage` arguments, please visit [Common Arguments](https://github.com/G1ANT-Robot/G1ANT.Manual/blob/master/G1ANT-Language/Common-Arguments.md) manual page.

This command is contained in **G1ANT.Language.dll.**

**Example 1:**

```G1ANT
break
```