---
title: Viper core
date: 2026-05-09
draft: false
---

Viper core is the part that knows how to read Viper code.

Right now `Viper_core` holds the grammar and a few helper functions for parsing files, resolving imports, getting type names, and collecting a whole program together before the interpreter or compiler runs it.

 ## What it accepts

A Viper file can have imports, functions, and statements.

```Vp
import "other.vp";

int main() {
    print("Hello");
    return 0;
}
```

Imports and functions are top level things.
Statements can be top level too, but if you define `main` then `main` is the entrypoint that gets ran.

 ## Parsing

The parser is made with Lark. When Viper cant parse a file it will show a `VP: Parse error`.

That usually means a missing semicolon `;`, a missing brace `{}` or `()`, or a statement that Viper doesnt know about yet.

 ## Program collection

Before running or compiling. Viper core walks through imports and collects all functions into one program.

It keeps:

`root_path` - The main file that started everything
`tree` - The parsed file tree
`functions` - Every function found in the main file and imports
`top_level_statements` - Statements from the root file only

Imported files can add functions. Top level statements from imported files dont get added to the root files top level statements.

 ## Helper functions

These are the main helpers in `Viper_core.language`.

`parse_source(source_code, filename)` parses text into a Viper tree.

`extract_string(token)` takes a string token like `"file.vp"` and returns the inside text.

`resolve_import_path(raw_path, importer_path)` figures out where an import points. Absolute imports stay absolute. Relative imports are based on the file thats doing the import.

`get_type_name(type_node)` turns the parser type node into the real Viper type name, like `string` becoming `str`.

`collect_program(root_path, source_code=None)` parses the root file, follows imports, blocks circular imports, blocks duplicate functions, and returns the full program data.
