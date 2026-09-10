# 微信小程序编译器 Linux arm64 版本

[![Build WeChat DevTools (ARM64)](https://github.com/Little-Data/wx-compiler-arm64/actions/workflows/build-arm64.yml/badge.svg)](https://github.com/Little-Data/wx-compiler-arm64/actions/workflows/build-arm64.yml)

# 原仓库

https://github.com/msojocs/wx-compiler

# 说明

本项目基于官方 Windows 版本运行逻辑实现。

# 实现思路

1. 使用 IDA 取得伪代码，与函数地址
2. 使用frida配合函数地址，对各个函数进行hook，参见 [frida-wx-compiler](https://github.com/msojocs/frida-wx-compiler)
3. 在Linux下根据伪代码复现逻辑，使用frida来校对函数处理前和处理后的数据是否符合实际

# 在找开发者工具的仓库？

[wechat-web-devtools-linux-arm64](https://github.com/Little-Data/wechat-web-devtools-linux-arm64)

开发者工具问题请到上面仓库反馈，本仓库只是开发者工具的编译器