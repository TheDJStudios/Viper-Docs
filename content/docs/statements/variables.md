---
title: Variable statements
date: 2026-05-09
draft: false
weight: 10
---

Variable statements make or edit variables.

 ## Make a variable

Start with `$`, then the name, then `:`, then the type, then `=`, then the value.

```Vp
$ count: int = 1;
```

You can read the variable with or without `$`.

```Vp
print(count);
print($count);
```

 ## Edit a variable

To edit a variable, use `$` then the name, then `=`.

```Vp
$ count: int = 1;

$ count = 2;
```

The new value still has to match the original type.
