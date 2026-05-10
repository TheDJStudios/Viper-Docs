---
title: Types
date: 2026-05-09
draft: false
weight: 20
---

Types tell Viper what kind of value a variable or function is supposed to use.

 ## Types

`int` Whole numbers
`float` Number that can have decimals
`double` Number that can have decimals
`str` Text
`string` Same as `str`
`char` One character
`bool` `true` or `false`
`none` No value
`void` Used for functions that dont return a value

There are also array type names:

`char[]`
`int[]`
`float[]`
`double[]`
`str[]`
`string[]`

These array types are in the core grammar. That means Viper can parse them as types.

 ## Example

```Vp
$ name: str = "Viper";
$ age: int = 1;
$ ready: bool = true;
```

Use `string` if you want, but Viper core treats it like `str`.
