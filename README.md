# QtGeo 🪐
> 一款基于 Qt 5.15 C++ 原生开发的跨平台动态几何绘图软件。专为统信 UOS 等国产 Linux 系统深度适配，无需 Wine 或虚拟机，开箱即用。

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Platform](https://img.shields.io/badge/Platform-UOS%20%7C%20Linux%20%7C%20Windows-lightgrey)]()
[![Framework](https://img.shields.io/badge/Qt-5.15-green)]()

## 📖 项目简介

随着统信 UOS 等国产操作系统的普及，许多经典的教育软件（如原版 GSP 几何画板）因底层架构原因无法直接运行。**QtGeo** 旨在打破这一壁垒，通过现代 C++ 与 Qt 框架，重构并致敬经典的动态几何画板。

本项目完全采用**原生代码**编写，确保在国产系统（DDE / X11 环境）上拥有丝滑的拖拽体验和精准的矢量绘图能力，免去配置 Wine 的繁琐与卡顿。

## ✨ 核心特性 (Features)

- 🖥️ **原生跨平台**：一套代码，完美运行于 UOS / Deepin / Windows。
- 📐 **动态几何依赖**：支持点、线、圆等几何对象的动态拖拽与父子级依赖传播更新。
- 📦 **免安装绿色包**：Linux 端提供独立打包（附带 Qt 依赖库），解压即用，**无需 sudo 权限**。
- 🎨 **现代 UI 渲染**：基于 `QGraphicsView` 框架与抗锯齿渲染，图形边缘平滑细腻。
- 🔤 **系统兼容**：全局默认采用 `Noto Sans SC`，适配国产系统显示规范。

## 🗺️ 开发路线图 (Roadmap)

项目目前正处于**核心架构搭建与逆向分析阶段**，欢迎持续关注：

- [x] 项目立项与 UOS 环境适配方案验证
- [ ] 提取并解析原版几何对象数据结构
- [ ] 实现基础几何内核（点、线段、圆、多边形）
- [ ] 实现动态几何父子依赖更新算法（Constraint Solver）
- [ ] 实现 Qt 画布交互与拖拽渲染
- [ ] UI 界面高保真重构
- [ ] 完成 UOS 平台免安装打包与 `.sh` 启动脚本
- [ ] 发布 v1.0.0 预览版本

## 🛠️ 构建与运行 (Build & Run)

### Windows / Linux 开发环境
- **IDE**: Qt Creator
- **Qt Version**: 5.15.2
- **Modules**: QtCore, QtGui, QtWidgets, QtSvg

*(项目代码正在火速开发中，构建指南将在首个可运行版本发布后更新)*

## ⚖️ 开源协议 (License)

本项目采用 **GNU General Public License v3.0 (GPLv3)** 协议开源。
你可以自由地运行、修改和分发本软件，但**必须保留原作者署名，且任何衍生作品必须同样以 GPLv3 协议开源**。

## ⚠️ 免责声明 (Disclaimer)

1. **非官方项目**：本项目为个人学习、技术研究与开源交流目的开发，与 McGraw-Hill（原几何画板母公司）无任何关联。
2. **纯净代码**：本项目**不包含**任何原版商业软件的二进制文件、反编译源码或受版权保护的 UI 素材。部分算法逻辑基于公开文件格式（`.gsp`）与学术论文进行独立重构。
3. **名称声明**：本项目尽量避免使用"几何画板"等可能涉及商标侵权的名称，旨在为教育工作者提供免费的替代方案。

## 🤝 贡献指南 (Contributing)

非常欢迎提交 Issue 或 Pull Request！
如果你对动态几何算法有研究，或者有 UOS 桌面端开发经验，欢迎加入一起完善这个项目。

---
*如果这个项目构想帮到了你，欢迎点个 ⭐ Star 支持一下！*
