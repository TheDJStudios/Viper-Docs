---
title: Try statements
date: 2026-05-09
draft: false
---

Try statements run a block and ignore Viper runtime errors from inside that block.

 ## Usage

```Vp
try {
    print(missingValue);
}

print("Still running");
```

In the interpreter, if code inside the `try` has a runtime error. Viper stops that try block and keeps going after it.

In the compiler, statements that fail while compiling inside a `try` block are skipped.
