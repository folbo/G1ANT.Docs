# Macro

## **Syntax**

```text
⊂//put some C# code here⊃
```

## **Description**

`⊂⊃` **Macro** allows to include C\# code between macro special characters which will get evaluated during the run and return result to your G1ANT variable. It is available at G1ANT Developer Studio -&gt; Insert -&gt; Macro. The shortcut for that is `Ctrl+9`.

### **Example** 1

In this example, we use C\# snippet to display current date and hour. In order to do this, we also convert this C\# data type to our G1ANT type – datetime.

```text
♥macro = ⟦datetime⟧⊂DateTime.Now⊃
dialog ♥macro
```

![](https://manula.r.sizr.io/large/user/7252/img/macro.png)

### Example 2

```text
♥initial_number = 9
♥factorial = ⊂(new Func<int, int>((n) => { int factorial = 1; for (int i = 1; i <= n; i++) factorial *= i; return factorial; })).Invoke(♥initial_number)⊃
dialog ♥factorial
```

In this example we are inserting a C\# macro code straight into G1ANT.Robot. We need to inject it between `⊂⊃`. Using delegates `(new Func<object,object>((x)=>{ x ...; x...; return x;})).Invoke(♥value)` is a method enabling the insertion of more statements into one macro. Inserting C\# macros is an advanced tool in G1ANT.Robot that expects prior knowledge of C\#.

