---
title: Variables
date: 2026-05-05
draft: false
---

Variables are useful for keeping info that needs to be used over and over again globally or locally. Such as getting a current state from another file to use in your current file. 
Heres an example:

```Vp
$ twopi: float = 3.14159 * 2;

print(twopi);
```

 ## Usage
 To use variables; You need to start the line with a `$`.

 To name a variable. Append the variable name after the `$` with a colon `:` directly after the name.
 such as `$ variablename:`.

 To set a variable type. Append one of the folowing types to right after the colon `:`
 `int`
 `double`
 `bool`
 `str`
 `none`

 like this:
 `$ variablename: double`
 Then, put a space then an equals sign `=`
 like this:
 `$ variablename: double =`
 And then finally. you want to give it a value.
 to do so. put a space after the equals sign `=` then put the value. make sure to end the line off with a semicolon `;`
 like this:
 `$ variablename: double = 3.14;`

 Then to use the variable:

 ```Vp
 $ variablename: double = 3.14;

 print(variablename);
 % or to use it in an if statement:

 if (variablename == 3.14) {
    print("Exactly pi");
 }
 ```