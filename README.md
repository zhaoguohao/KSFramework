# KSFramework
**K**Engine + **S**Lua + **Framework** = KSFramework

KSFramework是一个整合KEngine、SLua和一些开发组件组成的全功能Unity 5开发框架，适合有一定规模的团队使用。

目前正在开发中...

# 教程

- [KEngine策划指南：配置表的编辑与编译](http://www.jianshu.com/p/ead1a148b504)


## Session会话模块

### 为什么要用Session？
TODO

## UI模块

- 快速导出当前编辑的UI
- 支持运行时热重载UI脚本
- UISession（会话）支持

# 工程建议

- 建议创建两个工程：code和product，一个用于代码编辑，一个用于美术编辑导出AssetBundle。

# 键盘快捷键

- Ctrl+Alt+E: 在编辑UI场景时，导出UI成AssetBundle
- Ctrl+Alt+R: 在运行时，热重载所有LuaUIController
- Ctrl+Alt+I: 在编辑器，打开Game.unity主运行场景
- Ctrl+Alt+O: 在编辑器，打开Ctrl+Alt+I前的一个场景

# Unity编辑器强化工具

- 编辑代码后，返回正在运行的游戏，强制停到正在运行的游戏，避免崩溃的出现

# 多语言

## 增加收集器


## KEngine和KSFramework

### 定位不一样

KEngine:为了减低Unity 4.x中AssetBundle的加载、打包复杂度；

KSFramework:一站式的开发框架，可以开箱即用，包含SLua。只支持Unity 5。

### 提供的模块不同

KEngine: 提供基础的资源加载（ResourceModule）功能，并以之为基础，增加配置表（SettingModule）、UI模块（UIModule）这两个核心模块；另外还有针对Unity 4.x的资源依赖打包模块。

KSFramework：基于KEngine的资源、UI、配置表模块，实现更直接的、面向具体项目的常用功能模块，并搭配SLua。
