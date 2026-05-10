---
title: If statements
date: 2026-04-07
draft: false
---

If statements can be used to run a chunk of code based off of if a value matches another value.

 ## Usage
 To use an if statement. Write the following:
 ```Vp
 if (Value1 == value2) {
    // code here
 }
 ```
 If you use the code above. replace value1 with the variable you want to check against. then replace value2 with the value you want to see if value1 matches.

 If your variable is a bool (`True` or `False`) then you want to use the following code:
 ```Vp
 if (Value1) {
    % code here
 }
 ```
Then if value1 is `True` then the code in your `if` statement will run. else it wont run.

 ## Else
 To use else. then put `else` at the `}` at the end of your `if` statement.
 then put another set of `{}` after it like this:
 `} else {}`
 Then put the code you wanna run within them. like this:
 ```vp
 if (twopi == 3.14159 * 2) {
    print("Hello there Pi");
 } else {
    print("No pi for you ;/");

 }
 ```

 ## Else If
 if you wanna use else if. then put a `if` between `else` and `{}`
 like this :
 ```vp
 if (twopi == 3.14159 * 2) {
    print("Hello there Pi");
 } else if (twopi == 67) {
    print("Go to hell");

 } else {
    print("No Pi for you :/");

 }
 ```
