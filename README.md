# balancity-gnu-linux-fix

Guide for running BalanCity on GNU+Linux operating systems.

## Guide

_Note: Files you copy/download must be compatible with your game architecture._

1. Install libgconf
2. Add this to launch options:
```sh
LD_LIBRARY_PATH=/path/to/pango-1.43/lib %command%
```
3. Run BalanCity.

_Note: Required pango library files are included in this repository and are not part of this repository nor made by authors of this repository._

## Optional fixes

### Failed to open NaCl IRT file "…/steamapps/common/BalanCity/nacl_irt.nexe": -4

Get that file from there: https://chromium.googlesource.com/chromium/reference_builds.

### ReferenceError: module is not defined

Extract and replace index.html from the package.nw with a [patch](module.patch) applied to it.
