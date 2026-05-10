---
title: Quick reference
date: 2026-05-09
draft: false
weight: 5
---

This is the short version of the Viper syntax.

## Variables

```Vp
$ count: int = 1;
$ count = 2;

print(count);
print($count);
```

## Types

| Type | Meaning |
| --- | --- |
| `int` | Whole number |
| `float` | Decimal number |
| `double` | Decimal number |
| `str` | Text |
| `string` | Same as `str` |
| `char` | One character |
| `bool` | `true` or `false` |
| `none` | No value |
| `void` | Function returns no value |

## Operators

| Operator | Meaning |
| --- | --- |
| `+` | Add |
| `-` | Subtract or make negative |
| `*` | Multiply |
| `/` | Divide |
| `=` | Assign a value |
| `==` | Equal to |
| `!=` | Not equal to |
| `<` | Less than |
| `<=` | Less than or equal to |
| `>` | Greater than |
| `>=` | Greater than or equal to |
| `and` | Both requirements must be true |

## If statements

```Vp
if (count > 0) {
    print("Positive");
}
```

## Functions

```Vp
int getNumber() {
    return 7;
}

void sayHello() {
    print("Hello");
}
```

Viper functions do not take arguments yet, so the parentheses stay empty.

## Imports

```Vp
import "other.vp";
```

Imports can add functions from another file. Top level statements from imported files do not get added to the root file.
