# build-plugin-shellexecasuser

Test fixture for [nsis-dev/build-plugin](https://github.com/nsis-dev/build-plugin).

**Covers:** C++ with COM and ATL (`atlbase.h`), so msvc only. `VistaTools.cxx` is `#include`d rather than compiled, so `sources` names the one `.cpp` instead of a glob that would match `.cxx` too.

**Changed from upstream:** Dropped the bundled `nsis/` Plugin API copy and prebuilt `.lib`s and the Visual Studio project files; `GWL_USERDATA` became `GWLP_USERDATA` so 64-bit builds.
