---
title: JetBrains setup
date: 2026-05-09
draft: false
---

This is for setting up the Viper JetBrains plugin in an IntelliJ based IDE. Such as IntelliJ IDEA, PyCharm, WebStorm, CLion, or another JetBrains IDE.

 ## Build the plugin

From the repo root:

```sh
cd jetbrains-plugin
./gradlew buildPlugin
```

The plugin zip will be made in:

```sh
jetbrains-plugin/build/distributions/
```

 ## Install it in the IDE

Open your JetBrains IDE.

1. Open `Settings` or `Preferences`
2. Go to `Plugins`
3. Click the gear icon
4. Choose `Install Plugin from Disk...`
5. Pick the zip from `jetbrains-plugin/build/distributions/`
6. Restart the IDE if it asks

 ## Run it for testing

If you are working on the plugin itself. Use:

```sh
cd jetbrains-plugin
./gradlew runIde
```

That opens a sandbox IDE so you can test without installing it into your normal IDE.

 ## Runtime details

The plugin can run and compile `.vp` files from the IDE.

It looks for Python 3 and the `lark` package. If `lark` is missing, the plugin can try to install it, or you can run:

```sh
python3 -m pip install --user lark
```

The plugin first looks for Viper runtime files inside the project. It checks for:

`Viper_compiler/main.py`
`Viper_interpreter/Viper/main.py`

If those arent in the project, it can sync runtime files from GitHub releases into the JetBrains system folder.

 ## Useful plugin features

`.vp` files open as Viper files instead of plain text.

You get highlighting for keywords, types, builtins, variables, function calls, strings, chars, numbers, bools, and comments.

You get snippets for `if`, `else if`, `else`, `try`, `print`, `collect`, `import`, variables, functions, and `main`.

You can run or compile from the Tools menu, editor popup, project view popup, or toolbar when a `.vp` file is selected.
