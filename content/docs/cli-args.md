---
title: Args
date: 2026-05-09
draft: false
weight: 110
---

Viper has two built in values for command line args.

`$argc` - How many args were passed to the program
`$args` - The args as a string array

 ## Usage

```Vp
print($argc);
print(#"Args count: [$argc]");
```

`$args` is a `str[]`.
Right now the core can parse it and the runtime can pass it around, but there isnt array indexing syntax yet.
