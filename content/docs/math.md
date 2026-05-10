---
title: Operators
date: 2026-05-05
draft: false
weight: 60
---

Operators are the symbols and words Viper uses to calculate values, compare values, assign values, and combine requirements.

## Arithmetic operators

Use arithmetic operators with numbers.

| Operator | Meaning |
| --- | --- |
| `+` | Add |
| `-` | Subtract |
| `*` | Multiply |
| `/` | Divide |

```Vp
$ total: int = 4 + 2;
$ difference: int = 4 - 2;
$ doubled: int = 4 * 2;
$ half: int = 4 / 2;
```

You can use parentheses when you want to make the order clear.

```Vp
$ total: int = (1 + 2) * 3;
```

## Negative values

Put `-` before a number or variable to make it negative.

```Vp
$ score: int = -10;
$ penalty: int = -score;
```

## Assignment

Use `=` when you are giving a variable a value.

```Vp
$ score: int = 10;
$ score = 12;
```

Use `==` when you are checking whether two values are equal.

```Vp
if (score == 12) {
    print("Score is 12");
}
```

## Comparison operators

Comparisons return a `bool`.

| Operator | Meaning |
| --- | --- |
| `==` | Equal to |
| `!=` | Not equal to |
| `<` | Less than |
| `<=` | Less than or equal to |
| `>` | Greater than |
| `>=` | Greater than or equal to |

```Vp
$ count: int = 3;

if (count > 0) {
    print("Count is positive");
}

if (count != 10) {
    print("Count is not 10");
}
```

`<`, `<=`, `>`, and `>=` are for numbers. `==` and `!=` can be used with values that are the same kind of value, like a string compared to another string or a bool compared to another bool.

## Boolean operators

Use `and` when both requirements need to be true.

```Vp
if (ready == true and count > 0) {
    print("Running");
}
```

If Viper adds more boolean operators later, they should be documented here too.
