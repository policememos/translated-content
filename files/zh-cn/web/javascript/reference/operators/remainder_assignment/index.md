---
title: Remainder assignment (%=)
slug: Web/JavaScript/Reference/Operators/Remainder_assignment
---
{{jsSidebar("Operators")}}

The remainder assignment operator (`%=`) divides a variable by the value of the right operand and assigns the remainder to the variable.

{{EmbedInteractiveExample("pages/js/expressions-remainder-assignment.html")}}

## 语法

```plain
Operator: x %= y
Meaning:  x  = x % y
```

## Examples

### Using remainder assignment

```js
// Assuming the following variable
//  bar = 5

bar %= 2     // 1
bar %= 'foo' // NaN
bar %= 0     // NaN
```

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- [Assignment operators in the JS guide](/zh-CN/docs/Web/JavaScript/Guide/Expressions_and_Operators#Assignment)
- [Remainder operator](/zh-CN/docs/Web/JavaScript/Reference/Operators/Remainder)
