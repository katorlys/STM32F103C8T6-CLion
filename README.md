# STM32F103C8T6-CLion
[![License](https://img.shields.io/badge/license-MPL%202.0-brightgreen?style=flat-square)](https://mozilla.org/MPL/2.0) [![Pull Requests](https://img.shields.io/github/issues-pr-closed/katorlys/STM32F103C8T6-CLion?style=flat-square)](https://github.com/katorlys/STM32F103C8T6-CLion/pulls) [![Issues](https://img.shields.io/github/issues-closed/katorlys/STM32F103C8T6-CLion?style=flat-square)](https://github.com/katorlys/STM32F103C8T6-CLion/issues) [![Lines](https://img.shields.io/tokei/lines/github/katorlys/STM32F103C8T6-CLion?style=flat-square)](https://github.com/katorlys/STM32F103C8T6-CLion)

## 简介
可直接在 CLion 中使用的 STM32F103C8T6 项目工程模板。  

**库类型:** STM32标准库  
**平台:** OpenOCD  
**调试器:** ST-Link  

*注: 启动文件由 STM32CubeMX 生成，因此若要将项目迁移到 Keil，需要把启动文件更换成 Keil 专用的，否则无法编译通过。*  


## 使用方法
1. 复制`Project`文件夹 (路径不能有中文)
2. 用 CLion 打开
3. 新建文件、修改文件名、删除文件时, 要重新加载 CMake 项目
4. 新建文件夹时, 记得重新加载 CMake 项目
5. 点击`构建`即可在`cmake-build-debug`文件夹中获取到编译后的文件 (`.elf`,`.bin`,`.hex`和`.map`都有)
6. 点击`运行`即可把编译后的文件通过ST-LINK下载到STM32中, 若此前未构建则会先构建再下载
7. 点击`调试`即可开始调试, 与 Keil MDK 一样
8. 发送项目文件给别人时, 可以把`cmake-build-debug`文件夹删除, 其它文件则不能删除

