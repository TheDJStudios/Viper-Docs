---
title: Values and literals
date: 2026-05-09
draft: false
weight: 30
---

Literals are values you write straight into the file.

 ## Numbers

Numbers can be whole numbers or decimal numbers.

```Vp
$ count: int = 10;
$ pi: double = 3.14;
```

 ## Strings

Use double quotes for strings.

```Vp
$ name: str = "Viper";
```

You can also use single quotes for strings if it has more than one character, or if its empty.

```Vp
$ text: str = 'hello';
$ empty: str = '';
```

 ## Characters

Single quotes with one character makes a `char`.

```Vp
$ letter: char = 'v';
```

 ## Bools and none

```Vp
$ ready: bool = true;
$ done: bool = false;
$ nothing: none = none;
```

 ## Interpolated strings

Put `#` before a string to make an interpolated string.
Then put a variable inside `[]`.

```Vp
$ name: str = "Viper";

print(#"Hello [name]");
```

You can use `$argc` and `$args` in there too.

```Vp
print(#"You gave [$argc] args");
```
