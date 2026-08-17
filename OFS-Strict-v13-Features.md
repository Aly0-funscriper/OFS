# OFS strict v13 custom source

This repository is the strict v13 source snapshot used for the custom OFS build.

Included custom behavior:

- Frame-accurate keyboard stepping for both forward and backward navigation.
- Right-drag rectangle selection with time and height bounds; `Ctrl` adds to the current rectangle selection.
- Rectangle-selection paste is isolated from the original left-click selection/paste workflow.
- `Ctrl+B` inserts a copied action segment at the selected anchors without replacing existing actions.
- Lnip/Rnip graph support and the related editor changes from the strict v10 lineage.

The repository intentionally contains source and checked-in runtime assets only. Build outputs, caches, archives, and crash dumps are excluded by `.gitignore`.

## Build (Windows)

Configure this CMake project with a C++17-capable Visual Studio toolchain and build the `OpenFunscripter` target. The original project documentation and dependency manifest remain in this repository.
