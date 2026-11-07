# Changelog

## 0.7.0 — highlight-only

- **Breaking (intent)**: the extension is now **syntax highlighting only**.
  The bundled Python runtime and all commands (`elench.run` / `check` / `cost` /
  `build` / …) were removed — the toolchain is moving to a C++ backend, so
  editor integration will be rebuilt on top of that instead.
- Package size: **12.2 MB → 57 KB**.
- Added extension icon and a file-icon theme for `.eln` / `.tu`.
- Publisher changed to `xiaohuo123212`.

## 0.6.x and earlier

Bundled a Python runtime mirror and registered editor commands; superseded by 0.7.0.
