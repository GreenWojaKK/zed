# GreenWojaKK/zed fork

This branch (`tpui/v1.26.2-slim-image`) is a fork of [zed-industries/zed](https://github.com/zed-industries/zed)
used by [TPUI](https://github.com/GreenWojaKK/TPUI) to depend on GPUI.

It is based on the Zed release v1.26.2 (`c4273271`). The original license files are kept unchanged.
GPUI and its crates are licensed under the Apache License 2.0 by Zed Industries.

## Changes from upstream

- `Cargo.toml` (workspace root): the `image` dependency drops the `bmp`, `dds`, `exr`, `ff`, `hdr`,
  `ico`, `pnm`, `qoi`, `rayon`, `tga` and `tiff` features and keeps `gif`, `jpeg`, `png` and `webp`.
  GPUI decodes only these formats directly or for clipboard conversion, and the smaller feature set
  reduces the size of applications built with GPUI.
- `FORK.md`: this file.

No GPUI source code is modified.
