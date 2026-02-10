# MINGW DLL Copy Helper

帮助复制 DLL 到 exe 的目录

用于在 Linux 平台交叉编译 Windows 软件，或在 Windows MINGW 环境中打包发布软件

## 用法

```bash
./dllcopy <exe_path> <dll_list_path>

export DLLPATH=path/to/folder1:path/to/folder2:... # 使用冒号分隔多个搜索路径
./dllcopy app.exe dll_deps.txt
```

其中 `<dll_list_path>` 格式为一行一个dll名字

例如

```
libstdc++-6.dll
libgcc_s_seh-1.dll
libwinpthread-1.dll
zlib1.dll
```
