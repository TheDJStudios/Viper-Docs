---
title: Return statements
date: 2026-05-09
draft: false
weight: 50
---

Return statements send a value back from a function.

 ## Usage

```Vp
int getNumber() {
    return 5;
}
```

The value you return should match the function type.

```Vp
str getName() {
    return "Viper";
}
```

Dont use `return` outside of a function. Viper will error.
