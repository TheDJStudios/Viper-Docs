---
title: Collect statements
date: 2026-05-09
draft: false
weight: 60
---

Collect is used to read input from the user.

 ## As a statement

```Vp
collect();
```

You can also give it a prompt.

```Vp
collect("Name: ");
```

When used as a statement, Viper reads the input but doesnt keep it.

 ## As a value

Use `collect()` in an expression if you want to keep what the user typed.

```Vp
$ name: str = collect("Name: ");

print(#"Hello [name]");
```

`collect` returns a `str`.
