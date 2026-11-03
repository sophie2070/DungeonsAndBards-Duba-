Package: imgui:x64-windows@1.92.9

**Host Environment**

- Host: x64-windows
- Compiler: MSVC 19.51.36260.0
- CMake Version: 4.4.4
-    vcpkg-tool version: 2026-09-26-51bf87ca6e9bf3e622d84ff323bd202ab1ca0c0b
    vcpkg-scripts version: 20ceb8adbf 2026-10-14 (3 weeks ago)

**To Reproduce**

`vcpkg install `

**Failure logs**

```
-- Note: imgui only supports static library linkage. Building static library.
-- Using cached ocornut-imgui-v1.92.9b.tar.gz
-- Cleaning sources at C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/src/v1.92.9b-6eb65f6775.clean. Use --editable to skip cleaning for the packages you specify.
-- Extracting source C:/Users/twirr/Codeprograms/vcpkg/downloads/ocornut-imgui-v1.92.9b.tar.gz
-- Using source at C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/src/v1.92.9b-6eb65f6775.clean
-- Configuring x64-windows
CMake Error at scripts/cmake/vcpkg_execute_required_process.cmake:127 (message):
    Command failed: C:\\Users\\twirr\\Codeprograms\\vcpkg\\downloads\\tools\\ninja-1.13.2-windows\\ninja.exe -v
    Working Directory: C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel/vcpkg-parallel-configure
    Error code: 1
    See logs for more information:
      C:\Users\twirr\Codeprograms\vcpkg\buildtrees\imgui\config-x64-windows-dbg-CMakeCache.txt.log
      C:\Users\twirr\Codeprograms\vcpkg\buildtrees\imgui\config-x64-windows-rel-CMakeCache.txt.log
      C:\Users\twirr\Codeprograms\vcpkg\buildtrees\imgui\config-x64-windows-dbg-CMakeConfigureLog.yaml.log
      C:\Users\twirr\Codeprograms\vcpkg\buildtrees\imgui\config-x64-windows-rel-CMakeConfigureLog.yaml.log
      C:\Users\twirr\Codeprograms\vcpkg\buildtrees\imgui\config-x64-windows-out.log

Call Stack (most recent call first):
  C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/share/vcpkg-cmake/vcpkg_cmake_configure.cmake:271 (vcpkg_execute_required_process)
  C:/Users/twirr/AppData/Local/vcpkg/registries/git-trees/0529e7d45250a7e9f73a7f4163658a0a263d4871/portfile.cmake:81 (vcpkg_cmake_configure)
  scripts/ports.cmake:209 (include)



```

<details><summary>C:\Users\twirr\Codeprograms\vcpkg\buildtrees\imgui\config-x64-windows-out.log</summary>

```
[1/2] "C:/Program Files/CMake/bin/cmake.exe" -E chdir "../../x64-windows-dbg" "C:/Program Files/CMake/bin/cmake.exe" "C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/src/v1.92.9b-6eb65f6775.clean" "-G" "Ninja" "-DCMAKE_BUILD_TYPE=Debug" "-DCMAKE_INSTALL_PREFIX=C:/Users/twirr/Codeprograms/vcpkg/packages/imgui_x64-windows/debug" "-DFETCHCONTENT_FULLY_DISCONNECTED=ON" "-DIMGUI_BUILD_ALLEGRO5_BINDING=OFF" "-DIMGUI_BUILD_ANDROID_BINDING=OFF" "-DIMGUI_BUILD_DX9_BINDING=OFF" "-DIMGUI_BUILD_DX10_BINDING=OFF" "-DIMGUI_BUILD_DX11_BINDING=OFF" "-DIMGUI_BUILD_DX12_BINDING=OFF" "-DIMGUI_BUILD_GLFW_BINDING=OFF" "-DIMGUI_BUILD_GLUT_BINDING=OFF" "-DIMGUI_BUILD_METAL_BINDING=OFF" "-DIMGUI_BUILD_OPENGL2_BINDING=OFF" "-DIMGUI_BUILD_OPENGL3_BINDING=OFF" "-DIMGUI_BUILD_OSX_BINDING=OFF" "-DIMGUI_BUILD_SDL3_BINDING=OFF" "-DIMGUI_BUILD_SDLGPU3_BINDING=OFF" "-DIMGUI_BUILD_SDL3_RENDERER_BINDING=OFF" "-DIMGUI_BUILD_VULKAN_BINDING=OFF" "-DIMGUI_BUILD_WIN32_BINDING=OFF" "-DIMGUI_BUILD_WEBGPU_BINDING=OFF" "-DIMGUI_FREETYPE=OFF" "-DIMGUI_FREETYPE_SVG=OFF" "-DIMGUI_USE_WCHAR32=OFF" "-DIMGUI_TEST_ENGINE=OFF" "-DCMAKE_MAKE_PROGRAM=C:\Users\twirr\Codeprograms\vcpkg\downloads\tools\ninja-1.13.2-windows\ninja.exe" "-DBUILD_SHARED_LIBS=OFF" "-DVCPKG_CHAINLOAD_TOOLCHAIN_FILE=C:/Users/twirr/Codeprograms/vcpkg/scripts/toolchains/windows.cmake" "-DVCPKG_TARGET_TRIPLET=x64-windows" "-DVCPKG_SET_CHARSET_FLAG=ON" "-DVCPKG_PLATFORM_TOOLSET=v145" "-DCMAKE_EXPORT_NO_PACKAGE_REGISTRY=ON" "-DCMAKE_FIND_PACKAGE_NO_PACKAGE_REGISTRY=ON" "-DCMAKE_FIND_PACKAGE_NO_SYSTEM_PACKAGE_REGISTRY=ON" "-DCMAKE_INSTALL_SYSTEM_RUNTIME_LIBS_SKIP=TRUE" "-DCMAKE_VERBOSE_MAKEFILE=ON" "-DVCPKG_APPLOCAL_DEPS=OFF" "-DCMAKE_TOOLCHAIN_FILE=C:/Users/twirr/Codeprograms/vcpkg/scripts/buildsystems/vcpkg.cmake" "-DCMAKE_ERROR_ON_ABSOLUTE_INSTALL_DESTINATION=ON" "-DVCPKG_CXX_FLAGS=" "-DVCPKG_CXX_FLAGS_RELEASE=" "-DVCPKG_CXX_FLAGS_DEBUG=" "-DVCPKG_C_FLAGS=" "-DVCPKG_C_FLAGS_RELEASE=" "-DVCPKG_C_FLAGS_DEBUG=" "-DVCPKG_CRT_LINKAGE=dynamic" "-DVCPKG_LINKER_FLAGS=" "-DVCPKG_LINKER_FLAGS_RELEASE=" "-DVCPKG_LINKER_FLAGS_DEBUG=" "-DVCPKG_TARGET_ARCHITECTURE=x64" "-DCMAKE_INSTALL_LIBDIR:STRING=lib" "-DCMAKE_INSTALL_BINDIR:STRING=bin" "-D_VCPKG_ROOT_DIR=C:/Users/twirr/Codeprograms/vcpkg" "-D_VCPKG_INSTALLED_DIR=C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed" "-DVCPKG_MANIFEST_INSTALL=OFF" "-DIMGUI_SKIP_HEADERS=ON"
FAILED: [code=1] ../../x64-windows-dbg/CMakeCache.txt 
...
Skipped 23 lines
...
    no such file or directory
    ninja: build stopped: subcommand failed.
    
    



  CMake will not be able to correctly generate this project.
Call Stack (most recent call first):
  CMakeLists.txt:2 (project)


-- Configuring incomplete, errors occurred!
[2/2] "C:/Program Files/CMake/bin/cmake.exe" -E chdir ".." "C:/Program Files/CMake/bin/cmake.exe" "C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/src/v1.92.9b-6eb65f6775.clean" "-G" "Ninja" "-DCMAKE_BUILD_TYPE=Release" "-DCMAKE_INSTALL_PREFIX=C:/Users/twirr/Codeprograms/vcpkg/packages/imgui_x64-windows" "-DFETCHCONTENT_FULLY_DISCONNECTED=ON" "-DIMGUI_BUILD_ALLEGRO5_BINDING=OFF" "-DIMGUI_BUILD_ANDROID_BINDING=OFF" "-DIMGUI_BUILD_DX9_BINDING=OFF" "-DIMGUI_BUILD_DX10_BINDING=OFF" "-DIMGUI_BUILD_DX11_BINDING=OFF" "-DIMGUI_BUILD_DX12_BINDING=OFF" "-DIMGUI_BUILD_GLFW_BINDING=OFF" "-DIMGUI_BUILD_GLUT_BINDING=OFF" "-DIMGUI_BUILD_METAL_BINDING=OFF" "-DIMGUI_BUILD_OPENGL2_BINDING=OFF" "-DIMGUI_BUILD_OPENGL3_BINDING=OFF" "-DIMGUI_BUILD_OSX_BINDING=OFF" "-DIMGUI_BUILD_SDL3_BINDING=OFF" "-DIMGUI_BUILD_SDLGPU3_BINDING=OFF" "-DIMGUI_BUILD_SDL3_RENDERER_BINDING=OFF" "-DIMGUI_BUILD_VULKAN_BINDING=OFF" "-DIMGUI_BUILD_WIN32_BINDING=OFF" "-DIMGUI_BUILD_WEBGPU_BINDING=OFF" "-DIMGUI_FREETYPE=OFF" "-DIMGUI_FREETYPE_SVG=OFF" "-DIMGUI_USE_WCHAR32=OFF" "-DIMGUI_TEST_ENGINE=OFF" "-DCMAKE_MAKE_PROGRAM=C:\Users\twirr\Codeprograms\vcpkg\downloads\tools\ninja-1.13.2-windows\ninja.exe" "-DBUILD_SHARED_LIBS=OFF" "-DVCPKG_CHAINLOAD_TOOLCHAIN_FILE=C:/Users/twirr/Codeprograms/vcpkg/scripts/toolchains/windows.cmake" "-DVCPKG_TARGET_TRIPLET=x64-windows" "-DVCPKG_SET_CHARSET_FLAG=ON" "-DVCPKG_PLATFORM_TOOLSET=v145" "-DCMAKE_EXPORT_NO_PACKAGE_REGISTRY=ON" "-DCMAKE_FIND_PACKAGE_NO_PACKAGE_REGISTRY=ON" "-DCMAKE_FIND_PACKAGE_NO_SYSTEM_PACKAGE_REGISTRY=ON" "-DCMAKE_INSTALL_SYSTEM_RUNTIME_LIBS_SKIP=TRUE" "-DCMAKE_VERBOSE_MAKEFILE=ON" "-DVCPKG_APPLOCAL_DEPS=OFF" "-DCMAKE_TOOLCHAIN_FILE=C:/Users/twirr/Codeprograms/vcpkg/scripts/buildsystems/vcpkg.cmake" "-DCMAKE_ERROR_ON_ABSOLUTE_INSTALL_DESTINATION=ON" "-DVCPKG_CXX_FLAGS=" "-DVCPKG_CXX_FLAGS_RELEASE=" "-DVCPKG_CXX_FLAGS_DEBUG=" "-DVCPKG_C_FLAGS=" "-DVCPKG_C_FLAGS_RELEASE=" "-DVCPKG_C_FLAGS_DEBUG=" "-DVCPKG_CRT_LINKAGE=dynamic" "-DVCPKG_LINKER_FLAGS=" "-DVCPKG_LINKER_FLAGS_RELEASE=" "-DVCPKG_LINKER_FLAGS_DEBUG=" "-DVCPKG_TARGET_ARCHITECTURE=x64" "-DCMAKE_INSTALL_LIBDIR:STRING=lib" "-DCMAKE_INSTALL_BINDIR:STRING=bin" "-D_VCPKG_ROOT_DIR=C:/Users/twirr/Codeprograms/vcpkg" "-D_VCPKG_INSTALLED_DIR=C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed" "-DVCPKG_MANIFEST_INSTALL=OFF"
FAILED: [code=1] ../CMakeCache.txt 
"C:/Program Files/CMake/bin/cmake.exe" -E chdir ".." "C:/Program Files/CMake/bin/cmake.exe" "C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/src/v1.92.9b-6eb65f6775.clean" "-G" "Ninja" "-DCMAKE_BUILD_TYPE=Release" "-DCMAKE_INSTALL_PREFIX=C:/Users/twirr/Codeprograms/vcpkg/packages/imgui_x64-windows" "-DFETCHCONTENT_FULLY_DISCONNECTED=ON" "-DIMGUI_BUILD_ALLEGRO5_BINDING=OFF" "-DIMGUI_BUILD_ANDROID_BINDING=OFF" "-DIMGUI_BUILD_DX9_BINDING=OFF" "-DIMGUI_BUILD_DX10_BINDING=OFF" "-DIMGUI_BUILD_DX11_BINDING=OFF" "-DIMGUI_BUILD_DX12_BINDING=OFF" "-DIMGUI_BUILD_GLFW_BINDING=OFF" "-DIMGUI_BUILD_GLUT_BINDING=OFF" "-DIMGUI_BUILD_METAL_BINDING=OFF" "-DIMGUI_BUILD_OPENGL2_BINDING=OFF" "-DIMGUI_BUILD_OPENGL3_BINDING=OFF" "-DIMGUI_BUILD_OSX_BINDING=OFF" "-DIMGUI_BUILD_SDL3_BINDING=OFF" "-DIMGUI_BUILD_SDLGPU3_BINDING=OFF" "-DIMGUI_BUILD_SDL3_RENDERER_BINDING=OFF" "-DIMGUI_BUILD_VULKAN_BINDING=OFF" "-DIMGUI_BUILD_WIN32_BINDING=OFF" "-DIMGUI_BUILD_WEBGPU_BINDING=OFF" "-DIMGUI_FREETYPE=OFF" "-DIMGUI_FREETYPE_SVG=OFF" "-DIMGUI_USE_WCHAR32=OFF" "-DIMGUI_TEST_ENGINE=OFF" "-DCMAKE_MAKE_PROGRAM=C:\Users\twirr\Codeprograms\vcpkg\downloads\tools\ninja-1.13.2-windows\ninja.exe" "-DBUILD_SHARED_LIBS=OFF" "-DVCPKG_CHAINLOAD_TOOLCHAIN_FILE=C:/Users/twirr/Codeprograms/vcpkg/scripts/toolchains/windows.cmake" "-DVCPKG_TARGET_TRIPLET=x64-windows" "-DVCPKG_SET_CHARSET_FLAG=ON" "-DVCPKG_PLATFORM_TOOLSET=v145" "-DCMAKE_EXPORT_NO_PACKAGE_REGISTRY=ON" "-DCMAKE_FIND_PACKAGE_NO_PACKAGE_REGISTRY=ON" "-DCMAKE_FIND_PACKAGE_NO_SYSTEM_PACKAGE_REGISTRY=ON" "-DCMAKE_INSTALL_SYSTEM_RUNTIME_LIBS_SKIP=TRUE" "-DCMAKE_VERBOSE_MAKEFILE=ON" "-DVCPKG_APPLOCAL_DEPS=OFF" "-DCMAKE_TOOLCHAIN_FILE=C:/Users/twirr/Codeprograms/vcpkg/scripts/buildsystems/vcpkg.cmake" "-DCMAKE_ERROR_ON_ABSOLUTE_INSTALL_DESTINATION=ON" "-DVCPKG_CXX_FLAGS=" "-DVCPKG_CXX_FLAGS_RELEASE=" "-DVCPKG_CXX_FLAGS_DEBUG=" "-DVCPKG_C_FLAGS=" "-DVCPKG_C_FLAGS_RELEASE=" "-DVCPKG_C_FLAGS_DEBUG=" "-DVCPKG_CRT_LINKAGE=dynamic" "-DVCPKG_LINKER_FLAGS=" "-DVCPKG_LINKER_FLAGS_RELEASE=" "-DVCPKG_LINKER_FLAGS_DEBUG=" "-DVCPKG_TARGET_ARCHITECTURE=x64" "-DCMAKE_INSTALL_LIBDIR:STRING=lib" "-DCMAKE_INSTALL_BINDIR:STRING=bin" "-D_VCPKG_ROOT_DIR=C:/Users/twirr/Codeprograms/vcpkg" "-D_VCPKG_INSTALLED_DIR=C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed" "-DVCPKG_MANIFEST_INSTALL=OFF"
-- The CXX compiler identification is MSVC 19.51.36260.0
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - failed
-- Check for working CXX compiler: C:/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/cl.exe
-- Check for working CXX compiler: C:/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/cl.exe - broken
CMake Error at C:/Program Files/CMake/share/cmake-4.4/Modules/CMakeTestCXXCompiler.cmake:71 (message):
  The C++ compiler

    "C:/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/cl.exe"

  is not able to compile a simple test program.

  It fails with the following output:

    Change Dir: 'C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel/CMakeFiles/CMakeScratch/TryCompile-h4oxwn'
    
    Run Build Command(s): C:\Users\twirr\Codeprograms\vcpkg\downloads\tools\ninja-1.13.2-windows\ninja.exe -v cmTC_a6135
    [1/2] "C:\Program Files\Microsoft Visual Studio\18\Community\VC\Tools\MSVC\14.51.36231\bin\Hostx64\x64\cl.exe"  /nologo /TP -D_MBCS  /nologo /DWIN32 /D_WINDOWS /utf-8 /GR /EHsc /MP   /MDd /Z7 /Ob0 /Od /RTC1  -MDd /showIncludes /FoCMakeFiles\cmTC_a6135.dir\testCXXCompiler.cxx.obj /FdCMakeFiles\cmTC_a6135.dir\ /FS -c C:\Users\twirr\Codeprograms\vcpkg\buildtrees\imgui\x64-windows-rel\CMakeFiles\CMakeScratch\TryCompile-h4oxwn\testCXXCompiler.cxx
    [2/2] C:\WINDOWS\system32\cmd.exe /C "cd . && "C:\Program Files\CMake\bin\cmake.exe" -E vs_link_exe --msvc-ver=1951 --intdir=CMakeFiles\cmTC_a6135.dir --rc=rc --mt=CMAKE_MT-NOTFOUND --manifests  -- "C:\Program Files\Microsoft Visual Studio\18\Community\VC\Tools\MSVC\14.51.36231\bin\Hostx64\x64\link.exe" /nologo CMakeFiles\cmTC_a6135.dir\testCXXCompiler.cxx.obj  /out:cmTC_a6135.exe /implib:cmTC_a6135.lib /pdb:cmTC_a6135.pdb /version:0.0 /machine:x64 /nologo /debug /INCREMENTAL /subsystem:console  kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib && cd ."
    FAILED: [code=4294967295] cmTC_a6135.exe 
    C:\WINDOWS\system32\cmd.exe /C "cd . && "C:\Program Files\CMake\bin\cmake.exe" -E vs_link_exe --msvc-ver=1951 --intdir=CMakeFiles\cmTC_a6135.dir --rc=rc --mt=CMAKE_MT-NOTFOUND --manifests  -- "C:\Program Files\Microsoft Visual Studio\18\Community\VC\Tools\MSVC\14.51.36231\bin\Hostx64\x64\link.exe" /nologo CMakeFiles\cmTC_a6135.dir\testCXXCompiler.cxx.obj  /out:cmTC_a6135.exe /implib:cmTC_a6135.lib /pdb:cmTC_a6135.pdb /version:0.0 /machine:x64 /nologo /debug /INCREMENTAL /subsystem:console  kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib && cd ."
    RC Pass 1: command "rc /fo CMakeFiles\cmTC_a6135.dir/manifest.res CMakeFiles\cmTC_a6135.dir/manifest.rc" failed (exit code 0) with the following output:
    no such file or directory
    ninja: build stopped: subcommand failed.
    
    



  CMake will not be able to correctly generate this project.
Call Stack (most recent call first):
  CMakeLists.txt:2 (project)


-- Configuring incomplete, errors occurred!
ninja: build stopped: subcommand failed.
```
</details>

<details><summary>C:\Users\twirr\Codeprograms\vcpkg\buildtrees\imgui\config-x64-windows-rel-CMakeCache.txt.log</summary>

```
# This is the CMakeCache file.
# For build in directory: c:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel
# It was generated by CMake: C:/Program Files/CMake/bin/cmake.exe
# You can edit this file to change values found and used by cmake.
# If you do not want to change any of the values, simply exit the editor.
# If you do want to change a value, simply edit, save, and exit the editor.
# The syntax for the file is as follows:
# KEY:TYPE=VALUE
# KEY is the name of a variable in the cache.
# TYPE is a hint to GUIs for the type of VALUE, DO NOT EDIT TYPE!.
# VALUE is the current value for the KEY.

########################
# EXTERNAL cache entries
########################

//Global default for the library type used by add_library() when
// no STATIC/SHARED keyword is given: SHARED if true, STATIC otherwise.
// Not defined by CMake itself; commonly exposed as an option()
// by projects.
BUILD_SHARED_LIBS:UNINITIALIZED=OFF

//Path to a program.
CMAKE_AR:FILEPATH=C:/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/lib.exe

//Choose the type of build, options are: None Debug Release RelWithDebInfo
// MinSizeRel ...
CMAKE_BUILD_TYPE:STRING=Release

CMAKE_CROSSCOMPILING:STRING=OFF

//CXX compiler
CMAKE_CXX_COMPILER:FILEPATH=C:/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/cl.exe

CMAKE_CXX_FLAGS:STRING=' /nologo /DWIN32 /D_WINDOWS /utf-8 /GR /EHsc /MP '

CMAKE_CXX_FLAGS_DEBUG:STRING='/MDd /Z7 /Ob0 /Od /RTC1 '

//Flags used by the CXX compiler during MINSIZEREL builds.
CMAKE_CXX_FLAGS_MINSIZEREL:STRING=/O1 /Ob1 /DNDEBUG

CMAKE_CXX_FLAGS_RELEASE:STRING='/MD /O2 /Oi /Gy /DNDEBUG /Z7 '

//Flags used by the CXX compiler during RELWITHDEBINFO builds.
CMAKE_CXX_FLAGS_RELWITHDEBINFO:STRING=/Zi /O2 /Ob1 /DNDEBUG

//Libraries linked by default with all C++ applications.
CMAKE_CXX_STANDARD_LIBRARIES:STRING=kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib

CMAKE_C_FLAGS:STRING=' /nologo /DWIN32 /D_WINDOWS /utf-8 /MP '

CMAKE_C_FLAGS_DEBUG:STRING='/MDd /Z7 /Ob0 /Od /RTC1 '

CMAKE_C_FLAGS_RELEASE:STRING='/MD /O2 /Oi /Gy /DNDEBUG /Z7 '

//Error when cmake_install.cmake encounters absolute INSTALL DESTINATION.
CMAKE_ERROR_ON_ABSOLUTE_INSTALL_DESTINATION:UNINITIALIZED=ON

//Flags used by the linker during all build types.
CMAKE_EXE_LINKER_FLAGS:STRING=/machine:x64

//Flags used by the linker during DEBUG builds.
CMAKE_EXE_LINKER_FLAGS_DEBUG:STRING=/nologo    /debug /INCREMENTAL

//Flags used by the linker during MINSIZEREL builds.
CMAKE_EXE_LINKER_FLAGS_MINSIZEREL:STRING=/INCREMENTAL:NO

CMAKE_EXE_LINKER_FLAGS_RELEASE:STRING='/nologo /DEBUG /INCREMENTAL:NO /OPT:REF /OPT:ICF  '

//Flags used by the linker during RELWITHDEBINFO builds.
CMAKE_EXE_LINKER_FLAGS_RELWITHDEBINFO:STRING=/debug /INCREMENTAL

//Enable/Disable output of build database during the build.
CMAKE_EXPORT_BUILD_DATABASE:BOOL=

//Enable/Disable output of compile commands during generation.
CMAKE_EXPORT_COMPILE_COMMANDS:BOOL=

//Disable the export(PACKAGE) command from writing to the user
// package registry when CMP0090 is not set to NEW.
CMAKE_EXPORT_NO_PACKAGE_REGISTRY:UNINITIALIZED=ON

//DEPRECATED: Use CMAKE_FIND_USE_PACKAGE_REGISTRY instead. When
// unset, find_package uses User Package Registry unless disabled.
// Ignored if CMAKE_FIND_USE_PACKAGE_REGISTRY is set.
CMAKE_FIND_PACKAGE_NO_PACKAGE_REGISTRY:UNINITIALIZED=ON

//DEPRECATED: Use CMAKE_FIND_USE_SYSTEM_PACKAGE_REGISTRY instead.
// When unset, find_package uses System Package Registry unless
// disabled. Ignored if CMAKE_FIND_USE_SYSTEM_PACKAGE_REGISTRY
// is set.
CMAKE_FIND_PACKAGE_NO_SYSTEM_PACKAGE_REGISTRY:UNINITIALIZED=ON

//Value Computed by CMake.
CMAKE_FIND_PACKAGE_REDIRECTS_DIR:STATIC=C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel/CMakeFiles/pkgRedirects

//No help, variable specified on the command line.
CMAKE_INSTALL_BINDIR:STRING=bin

//No help, variable specified on the command line.
CMAKE_INSTALL_LIBDIR:STRING=lib

//Install path prefix, prepended onto install directories.
CMAKE_INSTALL_PREFIX:PATH=C:/Users/twirr/Codeprograms/vcpkg/packages/imgui_x64-windows

//No help, variable specified on the command line.
CMAKE_INSTALL_SYSTEM_RUNTIME_LIBS_SKIP:UNINITIALIZED=TRUE

//Path to a program.
CMAKE_LINKER:FILEPATH=C:/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/link.exe

//Tool that can launch the native build system. The value may be
// the full path to an executable or just the tool name if it is
...
Skipped 239 lines
...
VCPKG_PLATFORM_TOOLSET:UNINITIALIZED=v145

//Appends the vcpkg paths to CMAKE_PREFIX_PATH, CMAKE_LIBRARY_PATH
// and CMAKE_FIND_ROOT_PATH so that vcpkg libraries/packages are
// found after toolchain/system libraries/packages.
VCPKG_PREFER_SYSTEM_LIBS:BOOL=OFF

//Enable the setup of CMAKE_PROGRAM_PATH to vcpkg paths
VCPKG_SETUP_CMAKE_PROGRAM_PATH:BOOL=ON

//No help, variable specified on the command line.
VCPKG_SET_CHARSET_FLAG:UNINITIALIZED=ON

//No help, variable specified on the command line.
VCPKG_TARGET_ARCHITECTURE:UNINITIALIZED=x64

//Vcpkg target triplet (ex. x86-windows)
VCPKG_TARGET_TRIPLET:STRING=x64-windows

//Trace calls to find_package()
VCPKG_TRACE_FIND_PACKAGE:BOOL=OFF

//Use applocal.ps1 instead of vcpkg z-applocal.
VCPKG_USE_LEGACY_APPLOCAL:BOOL=OFF

//Enables messages from the VCPKG toolchain for debugging purposes.
VCPKG_VERBOSE:BOOL=OFF

//(experimental) Automatically copy dependencies into the install
// target directory for executables. Requires CMake 3.14.
X_VCPKG_APPLOCAL_DEPS_INSTALL:BOOL=OFF

//(experimental) Add USES_TERMINAL to VCPKG_APPLOCAL_DEPS to force
// serialization.
X_VCPKG_APPLOCAL_DEPS_SERIALIZED:BOOL=OFF

//The directory which contains the installed libraries for each
// triplet
_VCPKG_INSTALLED_DIR:PATH=C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed

//No help, variable specified on the command line.
_VCPKG_ROOT_DIR:UNINITIALIZED=C:/Users/twirr/Codeprograms/vcpkg

//Value Computed by CMake
imgui_BINARY_DIR:STATIC=C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel

//Value Computed by CMake
imgui_IS_TOP_LEVEL:STATIC=ON

//Value Computed by CMake
imgui_SOURCE_DIR:STATIC=C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/src/v1.92.9b-6eb65f6775.clean


########################
# INTERNAL cache entries
########################

//ADVANCED property for variable: CMAKE_AR
CMAKE_AR-ADVANCED:INTERNAL=1
//This is the directory where this CMakeCache.txt was created
CMAKE_CACHEFILE_DIR:INTERNAL=c:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel
//Major version of cmake used to create the current loaded cache
CMAKE_CACHE_MAJOR_VERSION:INTERNAL=4
//Minor version of cmake used to create the current loaded cache
CMAKE_CACHE_MINOR_VERSION:INTERNAL=4
//Patch version of cmake used to create the current loaded cache
CMAKE_CACHE_PATCH_VERSION:INTERNAL=4
//Path to CMake executable.
CMAKE_COMMAND:INTERNAL=C:/Program Files/CMake/bin/cmake.exe
//Path to cpack program executable.
CMAKE_CPACK_COMMAND:INTERNAL=C:/Program Files/CMake/bin/cpack.exe
//Path to ctest program executable.
CMAKE_CTEST_COMMAND:INTERNAL=C:/Program Files/CMake/bin/ctest.exe
//ADVANCED property for variable: CMAKE_CXX_COMPILER
CMAKE_CXX_COMPILER-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_FLAGS
CMAKE_CXX_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_FLAGS_DEBUG
CMAKE_CXX_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_FLAGS_MINSIZEREL
CMAKE_CXX_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_FLAGS_RELEASE
CMAKE_CXX_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_FLAGS_RELWITHDEBINFO
CMAKE_CXX_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_STANDARD_LIBRARIES
CMAKE_CXX_STANDARD_LIBRARIES-ADVANCED:INTERNAL=1
//Set initial state for CMake diagnostics; used to persist state
// set by command-line options across invocations.
CMAKE_DIAGNOSTIC_INIT:INTERNAL=CMD_AUTHOR=WARN;CMD_DEPRECATED=WARN;CMD_EXPERIMENTAL=WARN;CMD_INSTALL_ABSOLUTE_DESTINATION=IGNORE;CMD_POLICY=WARN;CMD_UNINITIALIZED=IGNORE;CMD_UNUSED_CLI=WARN
//Path to cache edit program executable.
CMAKE_EDIT_COMMAND:INTERNAL=C:/Program Files/CMake/bin/cmake-gui.exe
//Deprecated.  Use -W[no-]error=deprecated instead.
CMAKE_ERROR_DEPRECATED:INTERNAL=OFF
//Executable file format
CMAKE_EXECUTABLE_FORMAT:INTERNAL=Unknown
//ADVANCED property for variable: CMAKE_EXE_LINKER_FLAGS
CMAKE_EXE_LINKER_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXE_LINKER_FLAGS_DEBUG
CMAKE_EXE_LINKER_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXE_LINKER_FLAGS_MINSIZEREL
CMAKE_EXE_LINKER_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXE_LINKER_FLAGS_RELEASE
CMAKE_EXE_LINKER_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXE_LINKER_FLAGS_RELWITHDEBINFO
CMAKE_EXE_LINKER_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXPORT_BUILD_DATABASE
CMAKE_EXPORT_BUILD_DATABASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXPORT_COMPILE_COMMANDS
CMAKE_EXPORT_COMPILE_COMMANDS-ADVANCED:INTERNAL=1
//Name of external makefile project generator.
CMAKE_EXTRA_GENERATOR:INTERNAL=
//Name of generator.
CMAKE_GENERATOR:INTERNAL=Ninja
//Generator instance identifier.
CMAKE_GENERATOR_INSTANCE:INTERNAL=
//Name of generator platform.
CMAKE_GENERATOR_PLATFORM:INTERNAL=
//Name of generator toolset.
CMAKE_GENERATOR_TOOLSET:INTERNAL=
//Source directory with the top level CMakeLists.txt file for this
// project
CMAKE_HOME_DIRECTORY:INTERNAL=C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/src/v1.92.9b-6eb65f6775.clean
//ADVANCED property for variable: CMAKE_LINKER
CMAKE_LINKER-ADVANCED:INTERNAL=1
//Name of CMakeLists files to read
CMAKE_LIST_FILE_NAME:INTERNAL=CMakeLists.txt
//ADVANCED property for variable: CMAKE_MODULE_LINKER_FLAGS
CMAKE_MODULE_LINKER_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_MODULE_LINKER_FLAGS_DEBUG
CMAKE_MODULE_LINKER_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_MODULE_LINKER_FLAGS_MINSIZEREL
CMAKE_MODULE_LINKER_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_MODULE_LINKER_FLAGS_RELEASE
CMAKE_MODULE_LINKER_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_MODULE_LINKER_FLAGS_RELWITHDEBINFO
CMAKE_MODULE_LINKER_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_MT
CMAKE_MT-ADVANCED:INTERNAL=1
//number of local generators
CMAKE_NUMBER_OF_MAKEFILES:INTERNAL=1
//Platform information initialized
CMAKE_PLATFORM_INFO_INITIALIZED:INTERNAL=1
//ADVANCED property for variable: CMAKE_POLICY_VERSION_MINIMUM
CMAKE_POLICY_VERSION_MINIMUM-ADVANCED:INTERNAL=1
//noop for ranlib
CMAKE_RANLIB:INTERNAL=:
//ADVANCED property for variable: CMAKE_RC_COMPILER
CMAKE_RC_COMPILER-ADVANCED:INTERNAL=1
CMAKE_RC_COMPILER_WORKS:INTERNAL=1
//ADVANCED property for variable: CMAKE_RC_FLAGS
CMAKE_RC_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_RC_FLAGS_DEBUG
CMAKE_RC_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_RC_FLAGS_MINSIZEREL
CMAKE_RC_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_RC_FLAGS_RELEASE
CMAKE_RC_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_RC_FLAGS_RELWITHDEBINFO
CMAKE_RC_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//Path to CMake installation.
CMAKE_ROOT:INTERNAL=C:/Program Files/CMake/share/cmake-4.4
//ADVANCED property for variable: CMAKE_SHARED_LINKER_FLAGS
CMAKE_SHARED_LINKER_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SHARED_LINKER_FLAGS_DEBUG
CMAKE_SHARED_LINKER_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SHARED_LINKER_FLAGS_MINSIZEREL
CMAKE_SHARED_LINKER_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SHARED_LINKER_FLAGS_RELEASE
CMAKE_SHARED_LINKER_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SHARED_LINKER_FLAGS_RELWITHDEBINFO
CMAKE_SHARED_LINKER_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SKIP_INSTALL_RPATH
CMAKE_SKIP_INSTALL_RPATH-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SKIP_RPATH
CMAKE_SKIP_RPATH-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_STATIC_LINKER_FLAGS
CMAKE_STATIC_LINKER_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_STATIC_LINKER_FLAGS_DEBUG
CMAKE_STATIC_LINKER_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_STATIC_LINKER_FLAGS_MINSIZEREL
CMAKE_STATIC_LINKER_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_STATIC_LINKER_FLAGS_RELEASE
CMAKE_STATIC_LINKER_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_STATIC_LINKER_FLAGS_RELWITHDEBINFO
CMAKE_STATIC_LINKER_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_TOOLCHAIN_FILE
CMAKE_TOOLCHAIN_FILE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_VERBOSE_MAKEFILE
CMAKE_VERBOSE_MAKEFILE-ADVANCED:INTERNAL=1
//Deprecated.  Use -W[no-]deprecated instead.
CMAKE_WARN_DEPRECATED:INTERNAL=ON
//Install the dependencies listed in your manifest:
//\n    If this is off, you will have to manually install your dependencies.
//\n    See https://github.com/microsoft/vcpkg/tree/master/docs/specifications/manifests.md
// for more info.
//\n
VCPKG_MANIFEST_INSTALL:INTERNAL=OFF
//ADVANCED property for variable: VCPKG_VERBOSE
VCPKG_VERBOSE-ADVANCED:INTERNAL=1
//Making sure VCPKG_MANIFEST_MODE doesn't change
Z_VCPKG_CHECK_MANIFEST_MODE:INTERNAL=OFF
//Vcpkg root directory
Z_VCPKG_ROOT_DIR:INTERNAL=C:/Users/twirr/Codeprograms/vcpkg

```
</details>

<details><summary>C:\Users\twirr\Codeprograms\vcpkg\buildtrees\imgui\config-x64-windows-dbg-CMakeCache.txt.log</summary>

```
# This is the CMakeCache file.
# For build in directory: c:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-dbg
# It was generated by CMake: C:/Program Files/CMake/bin/cmake.exe
# You can edit this file to change values found and used by cmake.
# If you do not want to change any of the values, simply exit the editor.
# If you do want to change a value, simply edit, save, and exit the editor.
# The syntax for the file is as follows:
# KEY:TYPE=VALUE
# KEY is the name of a variable in the cache.
# TYPE is a hint to GUIs for the type of VALUE, DO NOT EDIT TYPE!.
# VALUE is the current value for the KEY.

########################
# EXTERNAL cache entries
########################

//Global default for the library type used by add_library() when
// no STATIC/SHARED keyword is given: SHARED if true, STATIC otherwise.
// Not defined by CMake itself; commonly exposed as an option()
// by projects.
BUILD_SHARED_LIBS:UNINITIALIZED=OFF

//Path to a program.
CMAKE_AR:FILEPATH=C:/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/lib.exe

//Choose the type of build, options are: None Debug Release RelWithDebInfo
// MinSizeRel ...
CMAKE_BUILD_TYPE:STRING=Debug

CMAKE_CROSSCOMPILING:STRING=OFF

//CXX compiler
CMAKE_CXX_COMPILER:FILEPATH=C:/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/cl.exe

CMAKE_CXX_FLAGS:STRING=' /nologo /DWIN32 /D_WINDOWS /utf-8 /GR /EHsc /MP '

CMAKE_CXX_FLAGS_DEBUG:STRING='/MDd /Z7 /Ob0 /Od /RTC1 '

//Flags used by the CXX compiler during MINSIZEREL builds.
CMAKE_CXX_FLAGS_MINSIZEREL:STRING=/O1 /Ob1 /DNDEBUG

CMAKE_CXX_FLAGS_RELEASE:STRING='/MD /O2 /Oi /Gy /DNDEBUG /Z7 '

//Flags used by the CXX compiler during RELWITHDEBINFO builds.
CMAKE_CXX_FLAGS_RELWITHDEBINFO:STRING=/Zi /O2 /Ob1 /DNDEBUG

//Libraries linked by default with all C++ applications.
CMAKE_CXX_STANDARD_LIBRARIES:STRING=kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib

CMAKE_C_FLAGS:STRING=' /nologo /DWIN32 /D_WINDOWS /utf-8 /MP '

CMAKE_C_FLAGS_DEBUG:STRING='/MDd /Z7 /Ob0 /Od /RTC1 '

CMAKE_C_FLAGS_RELEASE:STRING='/MD /O2 /Oi /Gy /DNDEBUG /Z7 '

//Error when cmake_install.cmake encounters absolute INSTALL DESTINATION.
CMAKE_ERROR_ON_ABSOLUTE_INSTALL_DESTINATION:UNINITIALIZED=ON

//Flags used by the linker during all build types.
CMAKE_EXE_LINKER_FLAGS:STRING=/machine:x64

//Flags used by the linker during DEBUG builds.
CMAKE_EXE_LINKER_FLAGS_DEBUG:STRING=/nologo    /debug /INCREMENTAL

//Flags used by the linker during MINSIZEREL builds.
CMAKE_EXE_LINKER_FLAGS_MINSIZEREL:STRING=/INCREMENTAL:NO

CMAKE_EXE_LINKER_FLAGS_RELEASE:STRING='/nologo /DEBUG /INCREMENTAL:NO /OPT:REF /OPT:ICF  '

//Flags used by the linker during RELWITHDEBINFO builds.
CMAKE_EXE_LINKER_FLAGS_RELWITHDEBINFO:STRING=/debug /INCREMENTAL

//Enable/Disable output of build database during the build.
CMAKE_EXPORT_BUILD_DATABASE:BOOL=

//Enable/Disable output of compile commands during generation.
CMAKE_EXPORT_COMPILE_COMMANDS:BOOL=

//Disable the export(PACKAGE) command from writing to the user
// package registry when CMP0090 is not set to NEW.
CMAKE_EXPORT_NO_PACKAGE_REGISTRY:UNINITIALIZED=ON

//DEPRECATED: Use CMAKE_FIND_USE_PACKAGE_REGISTRY instead. When
// unset, find_package uses User Package Registry unless disabled.
// Ignored if CMAKE_FIND_USE_PACKAGE_REGISTRY is set.
CMAKE_FIND_PACKAGE_NO_PACKAGE_REGISTRY:UNINITIALIZED=ON

//DEPRECATED: Use CMAKE_FIND_USE_SYSTEM_PACKAGE_REGISTRY instead.
// When unset, find_package uses System Package Registry unless
// disabled. Ignored if CMAKE_FIND_USE_SYSTEM_PACKAGE_REGISTRY
// is set.
CMAKE_FIND_PACKAGE_NO_SYSTEM_PACKAGE_REGISTRY:UNINITIALIZED=ON

//Value Computed by CMake.
CMAKE_FIND_PACKAGE_REDIRECTS_DIR:STATIC=C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-dbg/CMakeFiles/pkgRedirects

//No help, variable specified on the command line.
CMAKE_INSTALL_BINDIR:STRING=bin

//No help, variable specified on the command line.
...
Skipped 290 lines
...

//The directory which contains the installed libraries for each
// triplet
_VCPKG_INSTALLED_DIR:PATH=C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed

//No help, variable specified on the command line.
_VCPKG_ROOT_DIR:UNINITIALIZED=C:/Users/twirr/Codeprograms/vcpkg

//Value Computed by CMake
imgui_BINARY_DIR:STATIC=C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-dbg

//Value Computed by CMake
imgui_IS_TOP_LEVEL:STATIC=ON

//Value Computed by CMake
imgui_SOURCE_DIR:STATIC=C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/src/v1.92.9b-6eb65f6775.clean


########################
# INTERNAL cache entries
########################

//ADVANCED property for variable: CMAKE_AR
CMAKE_AR-ADVANCED:INTERNAL=1
//This is the directory where this CMakeCache.txt was created
CMAKE_CACHEFILE_DIR:INTERNAL=c:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-dbg
//Major version of cmake used to create the current loaded cache
CMAKE_CACHE_MAJOR_VERSION:INTERNAL=4
//Minor version of cmake used to create the current loaded cache
CMAKE_CACHE_MINOR_VERSION:INTERNAL=4
//Patch version of cmake used to create the current loaded cache
CMAKE_CACHE_PATCH_VERSION:INTERNAL=4
//Path to CMake executable.
CMAKE_COMMAND:INTERNAL=C:/Program Files/CMake/bin/cmake.exe
//Path to cpack program executable.
CMAKE_CPACK_COMMAND:INTERNAL=C:/Program Files/CMake/bin/cpack.exe
//Path to ctest program executable.
CMAKE_CTEST_COMMAND:INTERNAL=C:/Program Files/CMake/bin/ctest.exe
//ADVANCED property for variable: CMAKE_CXX_COMPILER
CMAKE_CXX_COMPILER-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_FLAGS
CMAKE_CXX_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_FLAGS_DEBUG
CMAKE_CXX_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_FLAGS_MINSIZEREL
CMAKE_CXX_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_FLAGS_RELEASE
CMAKE_CXX_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_FLAGS_RELWITHDEBINFO
CMAKE_CXX_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_CXX_STANDARD_LIBRARIES
CMAKE_CXX_STANDARD_LIBRARIES-ADVANCED:INTERNAL=1
//Set initial state for CMake diagnostics; used to persist state
// set by command-line options across invocations.
CMAKE_DIAGNOSTIC_INIT:INTERNAL=CMD_AUTHOR=WARN;CMD_DEPRECATED=WARN;CMD_EXPERIMENTAL=WARN;CMD_INSTALL_ABSOLUTE_DESTINATION=IGNORE;CMD_POLICY=WARN;CMD_UNINITIALIZED=IGNORE;CMD_UNUSED_CLI=WARN
//Path to cache edit program executable.
CMAKE_EDIT_COMMAND:INTERNAL=C:/Program Files/CMake/bin/cmake-gui.exe
//Deprecated.  Use -W[no-]error=deprecated instead.
CMAKE_ERROR_DEPRECATED:INTERNAL=OFF
//Executable file format
CMAKE_EXECUTABLE_FORMAT:INTERNAL=Unknown
//ADVANCED property for variable: CMAKE_EXE_LINKER_FLAGS
CMAKE_EXE_LINKER_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXE_LINKER_FLAGS_DEBUG
CMAKE_EXE_LINKER_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXE_LINKER_FLAGS_MINSIZEREL
CMAKE_EXE_LINKER_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXE_LINKER_FLAGS_RELEASE
CMAKE_EXE_LINKER_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXE_LINKER_FLAGS_RELWITHDEBINFO
CMAKE_EXE_LINKER_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXPORT_BUILD_DATABASE
CMAKE_EXPORT_BUILD_DATABASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_EXPORT_COMPILE_COMMANDS
CMAKE_EXPORT_COMPILE_COMMANDS-ADVANCED:INTERNAL=1
//Name of external makefile project generator.
CMAKE_EXTRA_GENERATOR:INTERNAL=
//Name of generator.
CMAKE_GENERATOR:INTERNAL=Ninja
//Generator instance identifier.
CMAKE_GENERATOR_INSTANCE:INTERNAL=
//Name of generator platform.
CMAKE_GENERATOR_PLATFORM:INTERNAL=
//Name of generator toolset.
CMAKE_GENERATOR_TOOLSET:INTERNAL=
//Source directory with the top level CMakeLists.txt file for this
// project
CMAKE_HOME_DIRECTORY:INTERNAL=C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/src/v1.92.9b-6eb65f6775.clean
//ADVANCED property for variable: CMAKE_LINKER
CMAKE_LINKER-ADVANCED:INTERNAL=1
//Name of CMakeLists files to read
CMAKE_LIST_FILE_NAME:INTERNAL=CMakeLists.txt
//ADVANCED property for variable: CMAKE_MODULE_LINKER_FLAGS
CMAKE_MODULE_LINKER_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_MODULE_LINKER_FLAGS_DEBUG
CMAKE_MODULE_LINKER_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_MODULE_LINKER_FLAGS_MINSIZEREL
CMAKE_MODULE_LINKER_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_MODULE_LINKER_FLAGS_RELEASE
CMAKE_MODULE_LINKER_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_MODULE_LINKER_FLAGS_RELWITHDEBINFO
CMAKE_MODULE_LINKER_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_MT
CMAKE_MT-ADVANCED:INTERNAL=1
//number of local generators
CMAKE_NUMBER_OF_MAKEFILES:INTERNAL=1
//Platform information initialized
CMAKE_PLATFORM_INFO_INITIALIZED:INTERNAL=1
//ADVANCED property for variable: CMAKE_POLICY_VERSION_MINIMUM
CMAKE_POLICY_VERSION_MINIMUM-ADVANCED:INTERNAL=1
//noop for ranlib
CMAKE_RANLIB:INTERNAL=:
//ADVANCED property for variable: CMAKE_RC_COMPILER
CMAKE_RC_COMPILER-ADVANCED:INTERNAL=1
CMAKE_RC_COMPILER_WORKS:INTERNAL=1
//ADVANCED property for variable: CMAKE_RC_FLAGS
CMAKE_RC_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_RC_FLAGS_DEBUG
CMAKE_RC_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_RC_FLAGS_MINSIZEREL
CMAKE_RC_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_RC_FLAGS_RELEASE
CMAKE_RC_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_RC_FLAGS_RELWITHDEBINFO
CMAKE_RC_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//Path to CMake installation.
CMAKE_ROOT:INTERNAL=C:/Program Files/CMake/share/cmake-4.4
//ADVANCED property for variable: CMAKE_SHARED_LINKER_FLAGS
CMAKE_SHARED_LINKER_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SHARED_LINKER_FLAGS_DEBUG
CMAKE_SHARED_LINKER_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SHARED_LINKER_FLAGS_MINSIZEREL
CMAKE_SHARED_LINKER_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SHARED_LINKER_FLAGS_RELEASE
CMAKE_SHARED_LINKER_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SHARED_LINKER_FLAGS_RELWITHDEBINFO
CMAKE_SHARED_LINKER_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SKIP_INSTALL_RPATH
CMAKE_SKIP_INSTALL_RPATH-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_SKIP_RPATH
CMAKE_SKIP_RPATH-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_STATIC_LINKER_FLAGS
CMAKE_STATIC_LINKER_FLAGS-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_STATIC_LINKER_FLAGS_DEBUG
CMAKE_STATIC_LINKER_FLAGS_DEBUG-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_STATIC_LINKER_FLAGS_MINSIZEREL
CMAKE_STATIC_LINKER_FLAGS_MINSIZEREL-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_STATIC_LINKER_FLAGS_RELEASE
CMAKE_STATIC_LINKER_FLAGS_RELEASE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_STATIC_LINKER_FLAGS_RELWITHDEBINFO
CMAKE_STATIC_LINKER_FLAGS_RELWITHDEBINFO-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_TOOLCHAIN_FILE
CMAKE_TOOLCHAIN_FILE-ADVANCED:INTERNAL=1
//ADVANCED property for variable: CMAKE_VERBOSE_MAKEFILE
CMAKE_VERBOSE_MAKEFILE-ADVANCED:INTERNAL=1
//Deprecated.  Use -W[no-]deprecated instead.
CMAKE_WARN_DEPRECATED:INTERNAL=ON
//Install the dependencies listed in your manifest:
//\n    If this is off, you will have to manually install your dependencies.
//\n    See https://github.com/microsoft/vcpkg/tree/master/docs/specifications/manifests.md
// for more info.
//\n
VCPKG_MANIFEST_INSTALL:INTERNAL=OFF
//ADVANCED property for variable: VCPKG_VERBOSE
VCPKG_VERBOSE-ADVANCED:INTERNAL=1
//Making sure VCPKG_MANIFEST_MODE doesn't change
Z_VCPKG_CHECK_MANIFEST_MODE:INTERNAL=OFF
//Vcpkg root directory
Z_VCPKG_ROOT_DIR:INTERNAL=C:/Users/twirr/Codeprograms/vcpkg

```
</details>

<details><summary>C:\Users\twirr\Codeprograms\vcpkg\buildtrees\imgui\config-x64-windows-rel-CMakeConfigureLog.yaml.log</summary>

```

---
events:
  -
    kind: "message-v1"
    backtrace:
      - "C:/Program Files/CMake/share/cmake-4.4/Modules/CMakeDetermineSystem.cmake:218 (message)"
      - "CMakeLists.txt:2 (project)"
    message: |
      The system is: Windows - 10.0.26200 - AMD64
  -
    kind: "find-v1"
    backtrace:
      - "C:/Program Files/CMake/share/cmake-4.4/Modules/CMakeDetermineCompiler.cmake:63 (find_program)"
      - "C:/Program Files/CMake/share/cmake-4.4/Modules/CMakeDetermineCXXCompiler.cmake:69 (_cmake_find_compiler)"
      - "CMakeLists.txt:2 (project)"
    mode: "program"
    variable: "CMAKE_CXX_COMPILER"
    description: "CXX compiler"
    settings:
      SearchFramework: "LAST"
      SearchAppBundle: "LAST"
      CMAKE_FIND_USE_CMAKE_PATH: false
      CMAKE_FIND_USE_CMAKE_ENVIRONMENT_PATH: false
      CMAKE_FIND_USE_SYSTEM_ENVIRONMENT_PATH: true
      CMAKE_FIND_USE_CMAKE_SYSTEM_PATH: false
      CMAKE_FIND_USE_INSTALL_PREFIX: true
    names:
      - "c++"
      - "g++"
      - "cl"
      - "bcc"
      - "icx"
      - "clang++"
    candidate_directories:
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/VC/vcpackages/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/CommonExtensions/Microsoft/TestWindow/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/CommonExtensions/Microsoft/TeamFoundation/Team Explorer/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files/Microsoft Visual Studio/18/Community/MSBuild/Current/Bin/Roslyn/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files (x86)/Microsoft SDKs/Windows/v10.0A/bin/NETFX 4.8 Tools/x64/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files/Microsoft Visual Studio/18/Community/Team Tools/DiagnosticsHub/Collector/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/Extensions/Microsoft/CodeCoverage.Console/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files/Microsoft Visual Studio/18/Community/MSBuild/Current/Bin/amd64/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Windows/Microsoft.NET/Framework64/v4.0.30319/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files/Microsoft Visual Studio/18/Community/Common7/Tools/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Users/twirr/Codeprograms/vcpkg/downloads/tools/powershell-core-7.6.6-windows/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Windows/System32/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Windows/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Windows/System32/wbem/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Windows/System32/WindowsPowerShell/v1.0/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Windows/System32/OpenSSH/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/VC/Linux/bin/ConnectionManagerExe/"
...
Skipped 2781 lines
...
    checks:
      - "Detecting CXX compiler ABI info"
    directories:
      source: "C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel/CMakeFiles/CMakeScratch/TryCompile-yewxuu"
      binary: "C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel/CMakeFiles/CMakeScratch/TryCompile-yewxuu"
    cmakeVariables:
      CMAKE_CXX_FLAGS: " /nologo /DWIN32 /D_WINDOWS /utf-8 /GR /EHsc /MP "
      CMAKE_CXX_FLAGS_DEBUG: "/MDd /Z7 /Ob0 /Od /RTC1 "
      CMAKE_CXX_SCAN_FOR_MODULES: "OFF"
      CMAKE_CXX_STDLIB_MODULES_JSON: ""
      CMAKE_EXE_LINKER_FLAGS: "/machine:x64"
      CMAKE_MSVC_DEBUG_INFORMATION_FORMAT: ""
      CMAKE_MSVC_RUNTIME_LIBRARY: "MultiThreaded$<$<CONFIG:Debug>:Debug>$<$<STREQUAL:dynamic,dynamic>:DLL>"
      VCPKG_CHAINLOAD_TOOLCHAIN_FILE: "C:/Users/twirr/Codeprograms/vcpkg/scripts/toolchains/windows.cmake"
      VCPKG_CRT_LINKAGE: "dynamic"
      VCPKG_CXX_FLAGS: ""
      VCPKG_CXX_FLAGS_DEBUG: ""
      VCPKG_CXX_FLAGS_RELEASE: ""
      VCPKG_C_FLAGS: ""
      VCPKG_C_FLAGS_DEBUG: ""
      VCPKG_C_FLAGS_RELEASE: ""
      VCPKG_INSTALLED_DIR: "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed"
      VCPKG_LINKER_FLAGS: ""
      VCPKG_LINKER_FLAGS_DEBUG: ""
      VCPKG_LINKER_FLAGS_RELEASE: ""
      VCPKG_PLATFORM_TOOLSET: "v145"
      VCPKG_PREFER_SYSTEM_LIBS: "OFF"
      VCPKG_SET_CHARSET_FLAG: "ON"
      VCPKG_TARGET_ARCHITECTURE: "x64"
      VCPKG_TARGET_TRIPLET: "x64-windows"
      Z_VCPKG_ROOT_DIR: "C:/Users/twirr/Codeprograms/vcpkg"
    buildResult:
      variable: "CMAKE_CXX_ABI_COMPILED"
      cached: false
      stdout: |
        Change Dir: 'C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel/CMakeFiles/CMakeScratch/TryCompile-yewxuu'
        
        Run Build Command(s): C:\\Users\\twirr\\Codeprograms\\vcpkg\\downloads\\tools\\ninja-1.13.2-windows\\ninja.exe -v cmTC_46cd4
        [1/2] "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\cl.exe"  /nologo /TP -D_MBCS  /nologo /DWIN32 /D_WINDOWS /utf-8 /GR /EHsc /MP   /MDd /Z7 /Ob0 /Od /RTC1  -MDd /showIncludes /FoCMakeFiles\\cmTC_46cd4.dir\\CMakeCXXCompilerABI.cpp.obj /FdCMakeFiles\\cmTC_46cd4.dir\\ /FS -c "C:\\Program Files\\CMake\\share\\cmake-4.4\\Modules\\CMakeCXXCompilerABI.cpp"
        [2/2] C:\\WINDOWS\\system32\\cmd.exe /C "cd . && "C:\\Program Files\\CMake\\bin\\cmake.exe" -E vs_link_exe --msvc-ver=1951 --intdir=CMakeFiles\\cmTC_46cd4.dir --rc=rc --mt=CMAKE_MT-NOTFOUND --manifests  -- "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\link.exe" /nologo CMakeFiles\\cmTC_46cd4.dir\\CMakeCXXCompilerABI.cpp.obj  /out:cmTC_46cd4.exe /implib:cmTC_46cd4.lib /pdb:cmTC_46cd4.pdb /version:0.0 /machine:x64 /nologo /debug /INCREMENTAL /subsystem:console  kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib && cd ."
        FAILED: [code=4294967295] cmTC_46cd4.exe 
        C:\\WINDOWS\\system32\\cmd.exe /C "cd . && "C:\\Program Files\\CMake\\bin\\cmake.exe" -E vs_link_exe --msvc-ver=1951 --intdir=CMakeFiles\\cmTC_46cd4.dir --rc=rc --mt=CMAKE_MT-NOTFOUND --manifests  -- "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\link.exe" /nologo CMakeFiles\\cmTC_46cd4.dir\\CMakeCXXCompilerABI.cpp.obj  /out:cmTC_46cd4.exe /implib:cmTC_46cd4.lib /pdb:cmTC_46cd4.pdb /version:0.0 /machine:x64 /nologo /debug /INCREMENTAL /subsystem:console  kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib && cd ."
        RC Pass 1: command "rc /fo CMakeFiles\\cmTC_46cd4.dir/manifest.res CMakeFiles\\cmTC_46cd4.dir/manifest.rc" failed (exit code 0) with the following output:
        no such file or directory
        ninja: build stopped: subcommand failed.
        
      exitCode: -1
  -
    kind: "try_compile-v1"
    backtrace:
      - "C:/Program Files/CMake/share/cmake-4.4/Modules/CMakeTestCXXCompiler.cmake:56 (try_compile)"
      - "CMakeLists.txt:2 (project)"
    checks:
      - "Check for working CXX compiler: C:/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/cl.exe"
    directories:
      source: "C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel/CMakeFiles/CMakeScratch/TryCompile-h4oxwn"
      binary: "C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel/CMakeFiles/CMakeScratch/TryCompile-h4oxwn"
    cmakeVariables:
      CMAKE_CXX_FLAGS: " /nologo /DWIN32 /D_WINDOWS /utf-8 /GR /EHsc /MP "
      CMAKE_CXX_FLAGS_DEBUG: "/MDd /Z7 /Ob0 /Od /RTC1 "
      CMAKE_CXX_SCAN_FOR_MODULES: "OFF"
      CMAKE_CXX_STDLIB_MODULES_JSON: ""
      CMAKE_EXE_LINKER_FLAGS: "/machine:x64"
      CMAKE_MSVC_DEBUG_INFORMATION_FORMAT: ""
      CMAKE_MSVC_RUNTIME_LIBRARY: "MultiThreaded$<$<CONFIG:Debug>:Debug>$<$<STREQUAL:dynamic,dynamic>:DLL>"
      VCPKG_CHAINLOAD_TOOLCHAIN_FILE: "C:/Users/twirr/Codeprograms/vcpkg/scripts/toolchains/windows.cmake"
      VCPKG_CRT_LINKAGE: "dynamic"
      VCPKG_CXX_FLAGS: ""
      VCPKG_CXX_FLAGS_DEBUG: ""
      VCPKG_CXX_FLAGS_RELEASE: ""
      VCPKG_C_FLAGS: ""
      VCPKG_C_FLAGS_DEBUG: ""
      VCPKG_C_FLAGS_RELEASE: ""
      VCPKG_INSTALLED_DIR: "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed"
      VCPKG_LINKER_FLAGS: ""
      VCPKG_LINKER_FLAGS_DEBUG: ""
      VCPKG_LINKER_FLAGS_RELEASE: ""
      VCPKG_PLATFORM_TOOLSET: "v145"
      VCPKG_PREFER_SYSTEM_LIBS: "OFF"
      VCPKG_SET_CHARSET_FLAG: "ON"
      VCPKG_TARGET_ARCHITECTURE: "x64"
      VCPKG_TARGET_TRIPLET: "x64-windows"
      Z_VCPKG_ROOT_DIR: "C:/Users/twirr/Codeprograms/vcpkg"
    buildResult:
      variable: "CMAKE_CXX_COMPILER_WORKS"
      cached: false
      stdout: |
        Change Dir: 'C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-rel/CMakeFiles/CMakeScratch/TryCompile-h4oxwn'
        
        Run Build Command(s): C:\\Users\\twirr\\Codeprograms\\vcpkg\\downloads\\tools\\ninja-1.13.2-windows\\ninja.exe -v cmTC_a6135
        [1/2] "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\cl.exe"  /nologo /TP -D_MBCS  /nologo /DWIN32 /D_WINDOWS /utf-8 /GR /EHsc /MP   /MDd /Z7 /Ob0 /Od /RTC1  -MDd /showIncludes /FoCMakeFiles\\cmTC_a6135.dir\\testCXXCompiler.cxx.obj /FdCMakeFiles\\cmTC_a6135.dir\\ /FS -c C:\\Users\\twirr\\Codeprograms\\vcpkg\\buildtrees\\imgui\\x64-windows-rel\\CMakeFiles\\CMakeScratch\\TryCompile-h4oxwn\\testCXXCompiler.cxx
        [2/2] C:\\WINDOWS\\system32\\cmd.exe /C "cd . && "C:\\Program Files\\CMake\\bin\\cmake.exe" -E vs_link_exe --msvc-ver=1951 --intdir=CMakeFiles\\cmTC_a6135.dir --rc=rc --mt=CMAKE_MT-NOTFOUND --manifests  -- "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\link.exe" /nologo CMakeFiles\\cmTC_a6135.dir\\testCXXCompiler.cxx.obj  /out:cmTC_a6135.exe /implib:cmTC_a6135.lib /pdb:cmTC_a6135.pdb /version:0.0 /machine:x64 /nologo /debug /INCREMENTAL /subsystem:console  kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib && cd ."
        FAILED: [code=4294967295] cmTC_a6135.exe 
        C:\\WINDOWS\\system32\\cmd.exe /C "cd . && "C:\\Program Files\\CMake\\bin\\cmake.exe" -E vs_link_exe --msvc-ver=1951 --intdir=CMakeFiles\\cmTC_a6135.dir --rc=rc --mt=CMAKE_MT-NOTFOUND --manifests  -- "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\link.exe" /nologo CMakeFiles\\cmTC_a6135.dir\\testCXXCompiler.cxx.obj  /out:cmTC_a6135.exe /implib:cmTC_a6135.lib /pdb:cmTC_a6135.pdb /version:0.0 /machine:x64 /nologo /debug /INCREMENTAL /subsystem:console  kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib && cd ."
        RC Pass 1: command "rc /fo CMakeFiles\\cmTC_a6135.dir/manifest.res CMakeFiles\\cmTC_a6135.dir/manifest.rc" failed (exit code 0) with the following output:
        no such file or directory
        ninja: build stopped: subcommand failed.
        
      exitCode: -1
...
```
</details>

<details><summary>C:\Users\twirr\Codeprograms\vcpkg\buildtrees\imgui\config-x64-windows-dbg-CMakeConfigureLog.yaml.log</summary>

```

---
events:
  -
    kind: "message-v1"
    backtrace:
      - "C:/Program Files/CMake/share/cmake-4.4/Modules/CMakeDetermineSystem.cmake:218 (message)"
      - "CMakeLists.txt:2 (project)"
    message: |
      The system is: Windows - 10.0.26200 - AMD64
  -
    kind: "find-v1"
    backtrace:
      - "C:/Program Files/CMake/share/cmake-4.4/Modules/CMakeDetermineCompiler.cmake:63 (find_program)"
      - "C:/Program Files/CMake/share/cmake-4.4/Modules/CMakeDetermineCXXCompiler.cmake:69 (_cmake_find_compiler)"
      - "CMakeLists.txt:2 (project)"
    mode: "program"
    variable: "CMAKE_CXX_COMPILER"
    description: "CXX compiler"
    settings:
      SearchFramework: "LAST"
      SearchAppBundle: "LAST"
      CMAKE_FIND_USE_CMAKE_PATH: false
      CMAKE_FIND_USE_CMAKE_ENVIRONMENT_PATH: false
      CMAKE_FIND_USE_SYSTEM_ENVIRONMENT_PATH: true
      CMAKE_FIND_USE_CMAKE_SYSTEM_PATH: false
      CMAKE_FIND_USE_INSTALL_PREFIX: true
    names:
      - "c++"
      - "g++"
      - "cl"
      - "bcc"
      - "icx"
      - "clang++"
    candidate_directories:
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/VC/vcpackages/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/CommonExtensions/Microsoft/TestWindow/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/CommonExtensions/Microsoft/TeamFoundation/Team Explorer/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files/Microsoft Visual Studio/18/Community/MSBuild/Current/Bin/Roslyn/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files (x86)/Microsoft SDKs/Windows/v10.0A/bin/NETFX 4.8 Tools/x64/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files/Microsoft Visual Studio/18/Community/Team Tools/DiagnosticsHub/Collector/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/Extensions/Microsoft/CodeCoverage.Console/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files/Microsoft Visual Studio/18/Community/MSBuild/Current/Bin/amd64/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Windows/Microsoft.NET/Framework64/v4.0.30319/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files/Microsoft Visual Studio/18/Community/Common7/Tools/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Users/twirr/Codeprograms/vcpkg/downloads/tools/powershell-core-7.6.6-windows/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Windows/System32/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Windows/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Windows/System32/wbem/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Windows/System32/WindowsPowerShell/v1.0/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Windows/System32/OpenSSH/"
      - "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed/x64-windows/debug/Program Files/Microsoft Visual Studio/18/Community/Common7/IDE/VC/Linux/bin/ConnectionManagerExe/"
...
Skipped 2780 lines
...
      - "CMakeLists.txt:2 (project)"
    checks:
      - "Detecting CXX compiler ABI info"
    directories:
      source: "C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-dbg/CMakeFiles/CMakeScratch/TryCompile-o046ei"
      binary: "C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-dbg/CMakeFiles/CMakeScratch/TryCompile-o046ei"
    cmakeVariables:
      CMAKE_CXX_FLAGS: " /nologo /DWIN32 /D_WINDOWS /utf-8 /GR /EHsc /MP "
      CMAKE_CXX_FLAGS_DEBUG: "/MDd /Z7 /Ob0 /Od /RTC1 "
      CMAKE_CXX_SCAN_FOR_MODULES: "OFF"
      CMAKE_CXX_STDLIB_MODULES_JSON: ""
      CMAKE_EXE_LINKER_FLAGS: "/machine:x64"
      CMAKE_MSVC_DEBUG_INFORMATION_FORMAT: ""
      CMAKE_MSVC_RUNTIME_LIBRARY: "MultiThreaded$<$<CONFIG:Debug>:Debug>$<$<STREQUAL:dynamic,dynamic>:DLL>"
      VCPKG_CHAINLOAD_TOOLCHAIN_FILE: "C:/Users/twirr/Codeprograms/vcpkg/scripts/toolchains/windows.cmake"
      VCPKG_CRT_LINKAGE: "dynamic"
      VCPKG_CXX_FLAGS: ""
      VCPKG_CXX_FLAGS_DEBUG: ""
      VCPKG_CXX_FLAGS_RELEASE: ""
      VCPKG_C_FLAGS: ""
      VCPKG_C_FLAGS_DEBUG: ""
      VCPKG_C_FLAGS_RELEASE: ""
      VCPKG_INSTALLED_DIR: "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed"
      VCPKG_LINKER_FLAGS: ""
      VCPKG_LINKER_FLAGS_DEBUG: ""
      VCPKG_LINKER_FLAGS_RELEASE: ""
      VCPKG_PLATFORM_TOOLSET: "v145"
      VCPKG_PREFER_SYSTEM_LIBS: "OFF"
      VCPKG_SET_CHARSET_FLAG: "ON"
      VCPKG_TARGET_ARCHITECTURE: "x64"
      VCPKG_TARGET_TRIPLET: "x64-windows"
      Z_VCPKG_ROOT_DIR: "C:/Users/twirr/Codeprograms/vcpkg"
    buildResult:
      variable: "CMAKE_CXX_ABI_COMPILED"
      cached: false
      stdout: |
        Change Dir: 'C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-dbg/CMakeFiles/CMakeScratch/TryCompile-o046ei'
        
        Run Build Command(s): C:\\Users\\twirr\\Codeprograms\\vcpkg\\downloads\\tools\\ninja-1.13.2-windows\\ninja.exe -v cmTC_9dd2c
        [1/2] "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\cl.exe"  /nologo /TP -D_MBCS  /nologo /DWIN32 /D_WINDOWS /utf-8 /GR /EHsc /MP   /MDd /Z7 /Ob0 /Od /RTC1  -MDd /showIncludes /FoCMakeFiles\\cmTC_9dd2c.dir\\CMakeCXXCompilerABI.cpp.obj /FdCMakeFiles\\cmTC_9dd2c.dir\\ /FS -c "C:\\Program Files\\CMake\\share\\cmake-4.4\\Modules\\CMakeCXXCompilerABI.cpp"
        [2/2] C:\\WINDOWS\\system32\\cmd.exe /C "cd . && "C:\\Program Files\\CMake\\bin\\cmake.exe" -E vs_link_exe --msvc-ver=1951 --intdir=CMakeFiles\\cmTC_9dd2c.dir --rc=rc --mt=CMAKE_MT-NOTFOUND --manifests  -- "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\link.exe" /nologo CMakeFiles\\cmTC_9dd2c.dir\\CMakeCXXCompilerABI.cpp.obj  /out:cmTC_9dd2c.exe /implib:cmTC_9dd2c.lib /pdb:cmTC_9dd2c.pdb /version:0.0 /machine:x64 /nologo /debug /INCREMENTAL /subsystem:console  kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib && cd ."
        FAILED: [code=4294967295] cmTC_9dd2c.exe 
        C:\\WINDOWS\\system32\\cmd.exe /C "cd . && "C:\\Program Files\\CMake\\bin\\cmake.exe" -E vs_link_exe --msvc-ver=1951 --intdir=CMakeFiles\\cmTC_9dd2c.dir --rc=rc --mt=CMAKE_MT-NOTFOUND --manifests  -- "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\link.exe" /nologo CMakeFiles\\cmTC_9dd2c.dir\\CMakeCXXCompilerABI.cpp.obj  /out:cmTC_9dd2c.exe /implib:cmTC_9dd2c.lib /pdb:cmTC_9dd2c.pdb /version:0.0 /machine:x64 /nologo /debug /INCREMENTAL /subsystem:console  kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib && cd ."
        RC Pass 1: command "rc /fo CMakeFiles\\cmTC_9dd2c.dir/manifest.res CMakeFiles\\cmTC_9dd2c.dir/manifest.rc" failed (exit code 0) with the following output:
        no such file or directory
        ninja: build stopped: subcommand failed.
        
      exitCode: -1
  -
    kind: "try_compile-v1"
    backtrace:
      - "C:/Program Files/CMake/share/cmake-4.4/Modules/CMakeTestCXXCompiler.cmake:56 (try_compile)"
      - "CMakeLists.txt:2 (project)"
    checks:
      - "Check for working CXX compiler: C:/Program Files/Microsoft Visual Studio/18/Community/VC/Tools/MSVC/14.51.36231/bin/Hostx64/x64/cl.exe"
    directories:
      source: "C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-dbg/CMakeFiles/CMakeScratch/TryCompile-lqgx9d"
      binary: "C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-dbg/CMakeFiles/CMakeScratch/TryCompile-lqgx9d"
    cmakeVariables:
      CMAKE_CXX_FLAGS: " /nologo /DWIN32 /D_WINDOWS /utf-8 /GR /EHsc /MP "
      CMAKE_CXX_FLAGS_DEBUG: "/MDd /Z7 /Ob0 /Od /RTC1 "
      CMAKE_CXX_SCAN_FOR_MODULES: "OFF"
      CMAKE_CXX_STDLIB_MODULES_JSON: ""
      CMAKE_EXE_LINKER_FLAGS: "/machine:x64"
      CMAKE_MSVC_DEBUG_INFORMATION_FORMAT: ""
      CMAKE_MSVC_RUNTIME_LIBRARY: "MultiThreaded$<$<CONFIG:Debug>:Debug>$<$<STREQUAL:dynamic,dynamic>:DLL>"
      VCPKG_CHAINLOAD_TOOLCHAIN_FILE: "C:/Users/twirr/Codeprograms/vcpkg/scripts/toolchains/windows.cmake"
      VCPKG_CRT_LINKAGE: "dynamic"
      VCPKG_CXX_FLAGS: ""
      VCPKG_CXX_FLAGS_DEBUG: ""
      VCPKG_CXX_FLAGS_RELEASE: ""
      VCPKG_C_FLAGS: ""
      VCPKG_C_FLAGS_DEBUG: ""
      VCPKG_C_FLAGS_RELEASE: ""
      VCPKG_INSTALLED_DIR: "C:/Users/twirr/personal projects/DnDNewApp/build/vcpkg_installed"
      VCPKG_LINKER_FLAGS: ""
      VCPKG_LINKER_FLAGS_DEBUG: ""
      VCPKG_LINKER_FLAGS_RELEASE: ""
      VCPKG_PLATFORM_TOOLSET: "v145"
      VCPKG_PREFER_SYSTEM_LIBS: "OFF"
      VCPKG_SET_CHARSET_FLAG: "ON"
      VCPKG_TARGET_ARCHITECTURE: "x64"
      VCPKG_TARGET_TRIPLET: "x64-windows"
      Z_VCPKG_ROOT_DIR: "C:/Users/twirr/Codeprograms/vcpkg"
    buildResult:
      variable: "CMAKE_CXX_COMPILER_WORKS"
      cached: false
      stdout: |
        Change Dir: 'C:/Users/twirr/Codeprograms/vcpkg/buildtrees/imgui/x64-windows-dbg/CMakeFiles/CMakeScratch/TryCompile-lqgx9d'
        
        Run Build Command(s): C:\\Users\\twirr\\Codeprograms\\vcpkg\\downloads\\tools\\ninja-1.13.2-windows\\ninja.exe -v cmTC_221ab
        [1/2] "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\cl.exe"  /nologo /TP -D_MBCS  /nologo /DWIN32 /D_WINDOWS /utf-8 /GR /EHsc /MP   /MDd /Z7 /Ob0 /Od /RTC1  -MDd /showIncludes /FoCMakeFiles\\cmTC_221ab.dir\\testCXXCompiler.cxx.obj /FdCMakeFiles\\cmTC_221ab.dir\\ /FS -c C:\\Users\\twirr\\Codeprograms\\vcpkg\\buildtrees\\imgui\\x64-windows-dbg\\CMakeFiles\\CMakeScratch\\TryCompile-lqgx9d\\testCXXCompiler.cxx
        [2/2] C:\\WINDOWS\\system32\\cmd.exe /C "cd . && "C:\\Program Files\\CMake\\bin\\cmake.exe" -E vs_link_exe --msvc-ver=1951 --intdir=CMakeFiles\\cmTC_221ab.dir --rc=rc --mt=CMAKE_MT-NOTFOUND --manifests  -- "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\link.exe" /nologo CMakeFiles\\cmTC_221ab.dir\\testCXXCompiler.cxx.obj  /out:cmTC_221ab.exe /implib:cmTC_221ab.lib /pdb:cmTC_221ab.pdb /version:0.0 /machine:x64 /nologo /debug /INCREMENTAL /subsystem:console  kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib && cd ."
        FAILED: [code=4294967295] cmTC_221ab.exe 
        C:\\WINDOWS\\system32\\cmd.exe /C "cd . && "C:\\Program Files\\CMake\\bin\\cmake.exe" -E vs_link_exe --msvc-ver=1951 --intdir=CMakeFiles\\cmTC_221ab.dir --rc=rc --mt=CMAKE_MT-NOTFOUND --manifests  -- "C:\\Program Files\\Microsoft Visual Studio\\18\\Community\\VC\\Tools\\MSVC\\14.51.36231\\bin\\Hostx64\\x64\\link.exe" /nologo CMakeFiles\\cmTC_221ab.dir\\testCXXCompiler.cxx.obj  /out:cmTC_221ab.exe /implib:cmTC_221ab.lib /pdb:cmTC_221ab.pdb /version:0.0 /machine:x64 /nologo /debug /INCREMENTAL /subsystem:console  kernel32.lib user32.lib gdi32.lib winspool.lib shell32.lib ole32.lib oleaut32.lib uuid.lib comdlg32.lib advapi32.lib && cd ."
        RC Pass 1: command "rc /fo CMakeFiles\\cmTC_221ab.dir/manifest.res CMakeFiles\\cmTC_221ab.dir/manifest.rc" failed (exit code 0) with the following output:
        no such file or directory
        ninja: build stopped: subcommand failed.
        
      exitCode: -1
...
```
</details>

**Additional context**

<details><summary>vcpkg.json</summary>

```
{
  "dependencies": [
    "portaudio",
    "imgui"
  ]
}

```
</details>
