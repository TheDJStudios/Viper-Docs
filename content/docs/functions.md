---
title: Functions
date: 2026-05-09
draft: false
weight: 80
---

Functions are named chunks of code you can call later.

 ## Usage

Start with the return type, then the function name, then `()` and a block.

```Vp
int getNumber() {
    return 7;
}

print(getNumber());
```

Viper functions dont take arguments yet. So the parentheses stay empty.

 ## Void functions

Use `void` if your function does something but doesnt return a value.

```Vp
void sayHello() {
    print("Hello");
}

sayHello();
```

 ## Main

If a function named `main` exists. Viper uses that as the entrypoint.

```Vp
int main() {
    print("Starting");
    return 0;
}
```

If theres no `main`, Viper runs the top level statements in the file.
