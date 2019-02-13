# dateformat

## Syntax

```G1ANT
♥dateformat = ⟦text⟧dd-MM-yyyy
```

## Description

Defines a date display format (eg. dd-MM-yyyy, dd.MM.yy, MM/dd/yy).

## Example

```G1ANT
♥dateformat = yyyy-MM-dd
dialog ♥date
♥dateformat = MM\/dd\/yy
dialog ♥date
```

This example shows current date in two different formats. If you want to use a slash (/) as a date separator, you should precede it with backslash (\\) as in the example above. Otherwise it will be ignored.
