# break

## Syntax

```G1ANT
break
```

## Description

The `break` command immediately exits current block and continues process execution.

| Argument | Type | Required | Default Value | Description |
| -------- | ---- | -------- | ------------- | ----------- |
| `if` | [bool](../structures/bool.md) | no | true | Executes the command only if a given condition is true |

For more information about the `if` argument, please see [Common Arguments](../appendices/common-arguments.md) page.

### Example

```G1ANT
for counter ♥cnt from 1 to 20
  if ⊂♥cnt==10⊃
    dialog ‴break‴    
    break
  end if 
end for
```

As you can see from the above example, `break` will only affect the `if` block command, not the `for` loop, which continues execution after the message dialog is closed.
