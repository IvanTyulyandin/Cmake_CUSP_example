# Cmake CUSP example

Minimal working example from CUSP library documentation.
Thrust/CUSP backend is OpenMP, see macros definition `THRUST_DEVICE_SYSTEM` in `main.cpp`.

## Prerequisites

[Thrust library, version 1.8.3](https://github.com/NVIDIA/thrust/releases/tag/1.8.3).

[CUSP library](https://github.com/cusplibrary/cusplibrary).

Required libraries are located in folders \<thrust-git-root/thrust> and \<cusp-git-root/cusp>.
These libraries are header-only, and can be placed at `/usr/local/include/thrust` and `/usr/local/include/cusp` accordingly.
