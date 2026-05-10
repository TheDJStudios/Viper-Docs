---
title: Imports
date: 2026-05-05
draft: false
weight: 100
---

Imports are used to include functions defined in other Viper files.
 ## Usage
 To import a file thats in the same directory; use the following:
 ```Vp
 import "import.vp";
 ```

 To import a file in a different directory; Use the following:
 ```vp
 import "/path/to/import.vp";
 ```

 Relative imports are based on the file that is doing the import.

 Imports are loaded before your main file keeps running. If two imported files define the same function, Viper will error since it wont know which one you mean.

 Also, dont import files in a circle. Like `a.vp` importing `b.vp` and `b.vp` importing `a.vp`. Viper will stop that with a circular import error.
