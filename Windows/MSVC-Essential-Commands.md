`CL.EXE` (2019)
===============


_Includes:_
-----------

`/I"<dir>"`  - add to include path  
`/X`         - ignore standard include places  

  
_Warnings:_
-----------

[`/experimental:external /external:anglebrackets /external:W0 /external:templates-`][external diagnostics] - disable warnings on system headers  
[`/experimental:external /analyze:external-`][external analysis] - shorter (and ~30% quicker?) version of above?  
[`/W3`][warning level]    - production quality warnings (use at least this)  
[`/W4`][warning level]    - informational warning level (lint-like)  
[`/Wall`][warning level]  - all warnings (/W4, including warnings that are off by default)  
[`/WX`][warning level]    - warnings as errors  
[`/sdl`][additional security]   - additional security warnings  
[`/analyze:plugin EspXEngine.dll`][guidelines checker] - enable c++ core guidelines checker  

[external diagnostics]: https://learn.microsoft.com/en-us/cpp/build/reference/external-external-headers-diagnostics?view=msvc-160
[external analysis]: https://learn.microsoft.com/en-us/cpp/build/reference/analyze-code-analysis?view=msvc-160#external-file-analysis-options
[warning level]: https://learn.microsoft.com/en-us/cpp/build/reference/compiler-option-warning-level?view=msvc-160
[additional security]: https://learn.microsoft.com/en-us/cpp/build/reference/sdl-enable-additional-security-checks?view=msvc-160
[guidelines checker]: https://learn.microsoft.com/en-us/cpp/code-quality/code-analysis-for-cpp-corecheck?view=msvc-160


_Optimizations:_
----------------

`/O2`        - maximum optimizations (favor speed)  
`/GA`        - optimize for windows application  
`/arch:`     - minimum cpu architecture: <`IA32` (xp) | `SSE` (pentium3) | `SSE2` (default) | `AVX` | `AVX2` | `AVX512`>  
`/F<bytes>`  - set stack size; nearest 4-byte multiple; default is 1 MB  


_Linking:_
----------

`/c`     - compile only, no link  
`/MD`    - msvcrt.lib (dynamically link c lib)  
`/MT`    - libcmt.lib (statically link c lib)  
`/LD`    - create .dll  
  
`/Fe`    - name executable file  
`/Fo`    - name object file  
  
`/link`  - linker options & libs  
`/link /LIBPATH:"<dir>"`           - add to lib path  
`/link /subsystem:console,"5.01"`  - x86 XP compatibility (<= v19.27)  
`/link /subsystem:console,"5.02"`  - x64 XP compatibility (<= v19.27)  
or  
`set _LINK_= -subsystem:console,"5.01"`  - sets env var for x86 XP (<= v19.27)  
`set _LINK_= -subsystem:console,"5.02"`  - sets env var for x64 XP (<= v19.27)  


_Debugging:_
------------

`/Od`    - disable optimizations (default)  
`/Za`    - disable extentions  
`/Zi`    - enable debug info  
`/MDd`   - msvcrt.lib (dynamic c debug lib)  
`/MTd`   - libcmt.lib (static c debug lib)  
`/LDd`   - create .dll debug lib  


_Other:_
--------

`/Zs`    - syntax check only  
`/P`     - preprocess to file  
`/C`     - don't strip comments  
`/FA`    - generate assembly listing  


_C++:_
------

`/TC`    - compile files as .c  
`/TP`    - compile files as .cpp  
`/std:`<`c++14` (default) | `c++17` | `c++latest`>  
`/EHsc`  - c++ error handling (no seh exceptions); `extern "C"` defaults to `nothrow`  


_`DUMPBIN.EXE`_
---------------

Check library dependencies:  
`dumpbin /dependents filename.exe`  

Check object bitness:  
`dumpbin /headers filename.exe |findstr machine`  


_MSBuild_
---------

`msbuild /m[:n] /p:platform=win32 /p:configuration=release /p:platformtoolset=v142 /t:clean`


_SDL2 (x86)_
------------

```cmd
cl.exe ^
    /arch:SSE ^
    /EHsc ^
    /I c:\path\to\sdl2\include ^
    *.c ^
    shell32.lib SDL2.lib SDL2main.lib SDL2_image.lib ^
    /link ^
    /libpath:c:\path\to\sdl2\lib\x86 ^
    /subsystem:console,"5.01"
```
