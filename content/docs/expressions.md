---
title: Expressions
date: 2026-05-09
draft: false
---

Expressions are values that Viper can figure out while running.

They can be plain values, variables, math, comparisons, function calls, `collect()`, or grouped values inside `()`.

 ## Usage

```Vp
$ count: int = 1 + 2;
$ bigger: bool = count > 2;

print(count);
```

You can put parentheses around expressions when you want to make the order clear.

```Vp
$ total: int = (1 + 2) * 3;
```

 ## Variables in expressions

Variables can be used with or without `$`.

```Vp
$ name: str = "Viper";

print(name);
print($name);
```

 ## Function calls in expressions

Functions that return a value can be used in expressions.

```Vp
int getCount() {
    return 3;
}

print(getCount() + 1);
```

Functions that return `void` need to be called as their own statement.
