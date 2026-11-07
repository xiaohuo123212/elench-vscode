# Elench for VS Code

Syntax highlighting and file icons for [Elench / Elenchus](https://github.com/xiaohuo123212/elench) —
a language where a **cost upper bound is part of the signature**.

| File | Meaning |
|---|---|
| `.tu` | contract (spec, `target`, `effects`, `requires`) |
| `.eln` | implementation |

## Install

From a VSIX (no marketplace account needed):

```bash
code --install-extension elench-0.7.0.vsix
```

Or in VS Code: `Extensions: Install from VSIX…`

## What it does — and does not

| | |
|---|---|
| ✅ Syntax highlighting (`.tu` / `.eln`) | grammar in `syntaxes/eln.tmLanguage.json` |
| ✅ Comments, brackets, auto-closing, indentation | `language-configuration.json` |
| ✅ File icons for `.eln` / `.tu` | `fileicons/elench-icon-theme.json` |
| ❌ No language server, no diagnostics | deliberate: the toolchain is moving to a C++ backend |

The command-line tool is separate — `npm install -g elench-lang` (the command is `elench`).

## Development

```bash
npx @vscode/vsce package      # produces elench-<version>.vsix
```

## License

Apache-2.0 — see `LICENSE`.
