
## [📖 Windows API](https://en.wikipedia.org/wiki/Windows_API)
* _Tutorials_
  - [Win32 API Programming Tutorial](http://www.winprog.org/tutorial/) - theForger
  - [Windows API tutorial](https://zetcode.com/gui/winapi/) - zetcode
  - [Windows Programming](https://en.wikibooks.org/wiki/Windows_Programming) - Wikibooks
* _Reference_
  - [Windows API Index](https://learn.microsoft.com/en-us/windows/win32/apiindex/windows-api-list) - Microsoft
    - [Windows Data Types](https://learn.microsoft.com/en-us/windows/win32/winprog/windows-data-types)
  - [Hungarian Notation](https://reactos.org/wiki/Hungarian_Notation) - ReactOS
  - [Win32 API (.chm)](https://web.archive.org/web/20190512102726id_/http://laurencejackson.com/win32/Win32.chm) - with arrows
  - [Win32 API (.hlp)](http://www.carabez.com/downloads/win32api.zip) - slim version
  - [Win32 API (.hlp)](http://www.carabez.com/downloads/win32api_big.zip) - big version


## ⚙️ Compilers
  * _MSVC_
    * __2015+__
      - [MSVC Essential Commands](MSVC-Essential-Commands.md)
      - [MSVC toolset at the command line](https://docs.microsoft.com/en-us/cpp/build/building-on-the-command-line) - Microsoft
      - [Download last XP-compatible MSVC v19.27 (Build Tools 2019 **\*\*\*v16.7.28\*\*\***)](https://download.visualstudio.microsoft.com/download/pr/2282640c-c74e-4d6a-9710-4eb8fef730e6/dfa5c24fb7aa4d11bf375bd2a46d19d3a1ff907cbc88468b0a50e3d71d53f77a/vs_BuildTools.exe)
      - [C/C++ language conformance by Visual Studio version](https://learn.microsoft.com/en-us/cpp/overview/visual-cpp-language-conformance?view=msvc-160)
    * __2010__
      - [PSDK 7.1](https://www.microsoft.com/en-us/download/details.aspx?id=8442)  
        _Includes C/C++ compiler and everything needed...  
        Uninstall ALL "Visual C++ 2010 Redistributables" from control panel FIRST!  
        Then burn/mount the image and run X:\Setup\SDKSetup.exe directly._
      - [C++0x Core Language Features In VC10: The Table](https://devblogs.microsoft.com/cppblog/c0x-core-language-features-in-vc10-the-table/)
      - [C++11 features in VC++ 2010 ](http://web.archive.org/web/20221127094629id_/https://learn.microsoft.com/en-us/previous-versions/hh567368(v=vs.140))
    * __2008__
      - [VS 2008 Express w/ SP1](https://download.microsoft.com/download/E/8/E/E8EEB394-7F42-4963-A2D8-29559B738298/VS2008ExpressWithSP1ENUX1504728.iso) - iso
      - [MSDN VS Express Library](web.archive.org/web/20190128091222id_/http://download.microsoft.com/download/9/9/5/995F050F-3E12-4A37-9B38-BEC3B3E899DA/msdnixp.exe)
      - [MSDN VS 2008 SP1 Library](http://download.microsoft.com/download/1/f/0/1f07c259-7ff2-4902-9205-ad1dfb87ccab/VS2008SP1MSDNENUX1506188.iso) - iso (standalone; won't integrate with express)
      - [VC++ Compiler for Python 2.7](http://web.archive.org/web/20160320053849id_/https://download.microsoft.com/download/7/9/6/796EF2E4-801B-4FC4-AB28-B59FBF6D907B/VCForPython27.msi)
    * __2005__
      - [VC++ 2005 Express Edition](http://go.microsoft.com/fwlink/?linkid=57034) - iso
        - [C++ doumentation](https://download.microsoft.com/download/1/6/d/16d24ada-5317-4de1-b2b2-890b51813d6e/VS2005_CPP_en-us.pdf) - pdf
        - [SDK documentation](https://download.microsoft.com/download/1/6/d/16d24ada-5317-4de1-b2b2-890b51813d6e/VS2005_SDK_en-us.pdf) - pdf
        - [General documentation](https://download.microsoft.com/download/1/6/d/16d24ada-5317-4de1-b2b2-890b51813d6e/VS2005_General_en-us.pdf) - pdf
    * __2003__
      - [VC++ 2003 Toolkit](https://archive.org/download/microsoft-visual-c-toolkit-2003/VCToolkitSetup.exe)  
        _Older alternative which will compile for Win9x/NT, as well..._  
      - [PSDK 2003 SP1](https://web.archive.org/web/20250508040615id_/https://download.microsoft.com/download/7/5/e/75ec7f04-4c8c-4f38-b582-966e76602643/5.2.3790.1830.15.PlatformSDK_Svr2003SP1_rtm.img)  
        _Install this with the 2003 toolkit._
      - [.NET Framework SDK Version 1.1](https://web.archive.org/web/20210820162511id_/https://download.microsoft.com/download/5/2/0/5202f918-306e-426d-9637-d7ee26fbe507/setup.exe)  
        _May be needed for a complete installation._
    * __6.0__
      - [SP5](https://archive.org/download/vs6sp5/vs6sp5.exe) - archive.org
        1. Edit `x:\path\to\sp598ent.stf` in `notepad.exe`
        2. On line starting with `13` delete the first `36`
      - [Processor Pack](http://download.microsoft.com/download/vb60ent/update/6/w9x2kxp/en-us/vcpp5.exe) - _(requires SP5)_ SSE / SSE2 / 3Dnow! / MASM 6.15
        _([readme](http://web.archive.org/web/20081222164354id_/http://msdn.microsoft.com/en-us/vs2005/aa718349.aspx))_
      - [vc6redistsetup_enu.exe](https://web.archive.org/web/20120610063726id_/http://download.microsoft.com/download/vc60pro/update/1/w9xnt4/en-us/vc6redistsetup_enu.exe)
    * __NMAKE__
      - [NMake 1.5](https://web.archive.org/web/20060615060342id_/http://download.microsoft.com/download/vc15/Patch/1.52/W95/EN-US/Nmake15.exe) - _32-bit (VC++ 2.0)_
      - [NMAKE Reference](https://learn.microsoft.com/en-us/cpp/build/reference/nmake-reference) - Microsoft
      - [Managing Projects with NMAKE](https://et.engr.iupui.edu/~dskim/downloadable/reference_Nmake.pdf)
  * _GCC_
    * __MSYS__
      - [MinGW/MSYS](https://sourceforge.net/projects/mingw/files/Installer) - x86 (only)
        - ~~Most recent (2017) [mingw-get-setup.exe](https://web.archive.org/web/20240225040417id_/https://osdn.dl.osdn.net/mingw/68260/mingw-get-setup.exe)~~
      - [MSYS2](https://www.msys2.org/) - x86 & x64
        - Last Windows 8.1 [installer](https://github.com/msys2/msys2-installer/releases/tag/2024-01-13)
        - Last Windows 7/8.0 [installer](https://github.com/msys2/msys2-installer/releases/tag/2022-10-28)
          - `$ pacman --noconfirm -Sy msys2-runtime-3.4 msys2-runtime-3.4-devel`
      - [TDM-GCC](https://jmeubank.github.io/tdm-gcc/)
    * __Dev-C++__
      - [Bloodshed](https://bloodshed.net/)
      - [wxDev](http://wxdsgn.sourceforge.net/)
      - [Orwell](https://orwelldevcpp.blogspot.com/)
      - [Embarcadero](https://github.com/Embarcadero/Dev-Cpp)
    * __POSIX Subsystem__
      - [Cygwin](https://www.cygwin.com/)
  * _BORLAND_
    * __C++ Builder__
      - [Borland C++ Compiler 5.5](https://altd.embarcadero.com/download/bcppbuilder/freecommandLinetools.exe) _(C++98)_
      - [Embarcadero C++ Compiler 7.30](https://altd.embarcadero.com/download/bcppbuilder/BCC102.zip) _(based on [clang](https://clang.llvm.org/)/[llvm](https://llvm.org/))_
  * _OTHERS_
    * [Orange C](https://ladsoft.tripod.com/orange_c_compiler.html) - LADSoft
    * [lcc-win](https://lcc-win32.services.net/) - Jacob Navia
    * [Smaller C](https://github.com/alexfru/SmallerC)
    * [Tiny C Compiler (TCC)](https://bellard.org/tcc/) - Fabrice Bellard


## ✔️ Design Guidelines
* [The Windows Interface Guidelines — A Guide for Designing Software](https://www.ics.uci.edu/~kobsa/courses/ICS104/course-notes/Microsoft_WindowsGuidelines.pdf) - Microsoft (1995)
* [Windows 7 Design Guidelines](https://learn.microsoft.com/en-us/windows/win32/uxguide/guidelines) - Microsoft
* [Windows 11 Design Guidelines](https://learn.microsoft.com/en-us/windows/apps/design/) - Microsoft


## 🔎 Debugging
* [Get started with WinDbg](https://github.com/MicrosoftDocs/windows-driver-docs/blob/staging/windows-driver-docs-pr/debugger/getting-started-with-windbg.md) - Microsoft
* [Windows Debuggers: A WinDbg Tutorial](https://www.codeproject.com/articles/6084/windows-debuggers-part-1-a-windbg-tutorial) - CodeProject


## 🩹 Exception Handling
* [Vectored Exception Handling in Windows XP](https://learn.microsoft.com/en-us/archive/msdn-magazine/2001/september/under-the-hood-new-vectored-exception-handling-in-windows-xp) - MSDN Magazine 2001
* [Depths of Win32 Structured Exception Handling](https://web.archive.org/web/20081230021224id_/http://www.microsoft.com/msj/0197/Exception/Exception.aspx) - Microsoft Systems Journal 1997
* [DWARF & SJLJ Exception Handling](https://gcc.gnu.org/wiki/WindowsGCCImprovements) - GCC
