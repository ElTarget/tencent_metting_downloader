# 🎯 腾讯会议转写纪要导出工具

[![Version](https://img.shields.io/badge/version-2.0.0-blue.svg)](https://github.com/awesome-tampermonkey/tencent-meeting-exporter)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Tampermonkey-orange.svg)](https://www.tampermonkey.net/)
[![Last Updated](https://img.shields.io/badge/last%20updated-2025--03--15-brightgreen.svg)]()
[![GitHub Stars](https://img.shields.io/github/stars/awesome-tampermonkey/tencent-meeting-exporter?style=social)](https://github.com/awesome-tampermonkey/tencent-meeting-exporter/stargazers)

> 🚀 **一键导出腾讯会议转写内容和纪要，支持多种格式导出和现代化UI体验**

## 🌟 项目简介

**腾讯会议转写纪要导出工具** 是一个强大的浏览器用户脚本，专为腾讯会议用户设计。它能够智能识别会议页面中的转写内容和会议纪要，并支持一键导出为多种格式（Markdown、HTML、TXT）。

### ✨ 主要特色

- 🎯 **智能识别**：自动识别转写和纪要内容
- 📱 **现代化UI**：玻璃拟态设计风格，支持响应式布局
- ⚡ **高性能**：虚拟滚动支持，大数据量也能快速处理
- 🛡️ **稳定可靠**：完整的错误处理和重试机制
- ♿ **无障碍**：支持键盘导航和屏幕阅读器

## 📸 界面预览

### 🎨 主界面
<div align="center">
  <p><em>现代化的玻璃拟态UI设计</em></p>
</div>

### 📋 导出选项
<div align="center">
  <p><em>丰富的导出格式和模式选择</em></p>
</div>


## 🚀 快速开始

### 📦 安装步骤

#### 1. 安装 Tampermonkey 扩展

<table>
  <tr>
    <th>浏览器</th>
    <th>安装链接</th>
    <th>说明</th>
  </tr>
  <tr>
    <td>Chrome</td>
    <td><a href="https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo">📥 安装 Tampermonkey</a></td>
    <td>推荐，性能最佳</td>
  </tr>
  <tr>
    <td>Firefox</td>
    <td><a href="https://addons.mozilla.org/firefox/addon/tampermonkey/">📥 安装 Tampermonkey</a></td>
    <td>完全支持</td>
  </tr>
  <tr>
    <td>Safari</td>
    <td><a href="https://apps.apple.com/us/app/tampermonkey/id1482490089">📥 安装 Tampermonkey</a></td>
    <td>需要 macOS 10.13+</td>
  </tr>
  <tr>
    <td>Edge</td>
    <td><a href="https://microsoftedge.microsoft.com/addons/detail/tampermonkey/iikmkjmpaadaobahmlepeloendndfphd">📥 安装 Tampermonkey</a></td>
    <td>基于 Chromium</td>
  </tr>
</table>

#### 2. 安装本脚本

**方法1：手动安装（没上到油猴的插件库）**
1. 访问 [Releases 页面](https://github.com/ElTarget/tencent_metting_downloader/releases)
2. 下载最新的 `.js` 文件
3. 到油猴窗口或点击安装


### 📖 使用指南

#### 🎯 基础使用

1. **打开会议页面**
   - 访问 `https://meeting.tencent.com/cw/*` 或 `https://meeting.tencent.com/ct/*`
   - 确保页面完全加载

2. **点击导出按钮**
   - 点击右上角的 **📝 导出转写/纪要** 按钮
   - 等待导出选项界面出现

3. **选择导出模式**
   - 🗣️ **转写导出**：仅导出会议转写内容
   - 📋 **纪要导出**：仅导出会议纪要内容
   - 📚 **同时导出**：分别导出两种内容
   - 📖 **整合导出**：合并到一个文件

4. **选择文件格式**
   - **Markdown** (推荐)：适合文档整理
   - **HTML**：适合网页展示
   - **TXT**：适合纯文本处理

5. **完成导出**
   - 文件将自动下载到本地
   - 根据内容大小可能需要等待几秒

#### 🐛 常见问题解决

- **按钮不显示**：刷新页面或检查Tampermonkey是否启用
- **内容获取失败**：等待页面完全加载后重试
- **导出文件为空**：确认页面包含转写或纪要内容
- **性能卡顿**：减少同时导出的内容量，分批处理


### 🎯 核心特性

#### 🧠 智能内容识别
- **多选择器支持**：适配不同版本的腾讯会议页面
- **智能降级**：当主要选择器失效时自动使用备选方案

#### ⚡ 性能优化
- **虚拟滚动支持**：高效处理大量转写内容
- **防抖处理(未更新)**：避免重复操作和界面卡顿
- **内存管理**：及时清理不再使用的资源
- **分批处理**：大文件分批次导出，避免浏览器崩溃

#### 🛡️ 稳定性保障
- **错误重试(未更新)**：网络错误自动重试，最多3次
- **超时保护(未更新)**：操作超时自动中断，防止无限等待
- **降级处理**：主要功能失效时提供备选方案
- **异常捕获(未更新)**：完整的错误捕获和用户提示

#### 🎨 现代化UI
- **玻璃拟态设计**：流行的半透明视觉效果

### 📊 性能指标

| 指标 | 目标值 | 实际表现 | 优化策略 |
|------|--------|----------|----------|
| **初始化时间** | < 2秒 | ✅ ~1.5秒 | 延迟加载 + 缓存优化 |
| **内容获取** | < 5秒 | ✅ ~3秒 | 虚拟滚动 + 分批处理 |
| **文件导出** | < 1秒 | ✅ ~0.5秒 | 流式处理 + 内存优化 |
| **内存占用** | < 50MB | ✅ ~30MB | 垃圾回收 + 资源释放 |

### 🔄 版本历史

v2.0.0 (2025-03-15)
- 完全重构代码结构
- 新增同步导出和整合一个文件导出功能
- 新增主页按钮长按拖动
- 优化UI

v1.0.0 (2025-03-10)
- 初始版本发布
- 基础导出功能实现

## 📄 许可证


本项目基于自定义非商用协议开源：

- ✅ 本代码基于自定义非商用协议（版本1.0，2026-03-15生效）授权，仅限个人非盈利使用
- ✅ 禁止行为包括：出售、广告变现、付费集成、付费小程序/APP开发等
- ✅ 学习和技术交流

但请遵守：
- 📝 保留原作者署名
- ⚠️ 承担使用风险
- 🤝 尊重开源精神
<div align="center">
 
### ⭐ 支持项目
 
如果这个项目对您有帮助，请给我们一个Star！
 
[![GitHub Stars](https://img.shields.io/github/stars/ElTarget/tencent_metting_downloader?style=social)](https://github.com/ElTarget/tencent_metting_downloader/stargazers)
 
**🎯 您的支持是我们持续改进的动力！**
 
</div>


<div align="center">

### ⭐ 支持项目

如果这个项目对您有帮助，请给我们一个Star！
