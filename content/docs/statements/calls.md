---
title: Function call statements
date: 2026-05-09
draft: false
weight: 40
---

Function calls run a function by name.

 ## Usage

```Vp
void sayHello() {
    print("Hello");
}

sayHello();
```

Function calls can also be used inside expressions if the function returns a value.

```Vp
int getNumber() {
    return 9;
}

print(getNumber());
```

If the function is `void`, call it as its own statement.
