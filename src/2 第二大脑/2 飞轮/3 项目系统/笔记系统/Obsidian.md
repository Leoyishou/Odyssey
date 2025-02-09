---
aliases: [Obsidian FastStart脚本使用指南]
draw:
tags: []
title: Obsidian FastStart脚本使用指南
date created: 2024-07-15
date modified: 2024-12-27
linter-yaml-title-alias: Obsidian FastStart脚本使用指南
---

## Obsidian FastStart脚本使用指南

### 背景介绍

Obsidian是一款以速度闻名的笔记软件，即使在较旧的设备上运行也很快。但是，当安装大量插件（25个或更多）时，应用程序的启动时间会变得较慢，特别是在移动设备上。

#### 为什么需要提高启动速度？

虽然PC上几秒钟的启动时间可以接受，但在移动设备上（如iPhone和iPad）5-8秒的启动时间会影响使用体验：

1. 移动设备内存有限，后台程序容易被系统卸载
2. 每次重新打开都需要完整加载
3. 启动延迟会造成使用摩擦，影响使用意愿

### FastStart脚本原理

#### Obsidian的启动过程

Obsidian启动时需要完成以下步骤：

1. 初始化内部内存缓存（保管库文件信息数据库）
2. 加载UI元素（按钮、窗格、工作区等）
3. 逐个加载已启用的插件

#### FastStart的工作方式

FastStart脚本通过以下方式优化启动速度：

1. 仅启用必要的核心插件进行启动
2. 快速完成初始化，使软件可用
3. 在后台分批延迟加载其他插件：
   - 第一批：启动2秒后加载
   - 第二批：启动30秒后加载

### 安装配置

#### 前期准备

1. 安装Templater插件
2. 设置Templater模板文件夹

#### 必要文件

需要创建以下文件：

1. `FastStart-StartupScript`（放在Templater文件夹中）
   - 包含主要JavaScript代码
   - 控制插件加载逻辑

2. `FastStart-GenerateListOfInstalledPlugins`（放在Templater文件夹中）
   - 用于生成已安装插件列表及ID

3. `FastStart-Plugins-ShortDelay`（可放在任意位置）
   - 存放需要短延迟加载的插件ID列表

4. `FastStart-Plugins-LongDelay`（可放在任意位置）
   - 存放需要长延迟加载的插件ID列表

#### 配置步骤

1. **配置Templater**
   - 在Templater设置中指定startup template
   - 选择FastStart-StartupScript作为启动脚本

2. **基准测试**
   - 记录当前启动时间作为基准
   - 测试安全模式下的最小启动时间

3. **插件分类**
   - 确定必须立即启动的插件（如Templater）
   - 规划短延迟加载的插件
   - 规划长延迟加载的插件

### 优化调试

#### 调试方法

1. 启用"Debug startup time"选项
2. 记录并对比不同配置下的启动时间
3. 测试不同插件组合的效果

#### 性能调优

1. 调整延迟时间（默认2秒和30秒）
2. 优化插件加载顺序
3. 处理特殊插件（某些插件可能不支持延迟加载）

### 最佳实践

1. 仔细评估每个插件的必要性
2. 将最常用的插件放入短延迟列表
3. 定期检查和调整插件配置
4. 为不同设备定制最佳延迟时间

### 注意事项

1. Templater插件必须保持启用状态
2. 某些插件可能需要立即启动
3. 调试过程需要反复测试和优化
4. 可能需要针对不同设备调整配置
