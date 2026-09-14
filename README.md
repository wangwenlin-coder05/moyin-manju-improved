# 🎬 Moyin Manju Improved · AI 影视生产工具（改良版）

> **⚠️ 本仓库为第三方改良版，非原创**——系在原项目基础之上进行的二次开发、Bug 修复与功能增强。

![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=for-the-badge&logo=typescript)
![Electron](https://img.shields.io/badge/Electron-28-47848F?style=for-the-badge&logo=electron)
![AI](https://img.shields.io/badge/AI-Video/Chat-D946EF?style=for-the-badge&logo=ai)
![Status](https://img.shields.io/badge/Status-改良版-FF6F00?style=for-the-badge)
![License](https://img.shields.io/badge/License-AGPL--3.0-blue?style=for-the-badge)

> AI 驱动的影视内容生产级工具：从剧本到成片的全流程批量化。支持 Seedance 2.0，一键完成分镜生成、视频合成、字幕对齐、配乐选择等环节，极大缩短 AI 短剧 / 漫剧的制作周期。

---

## ✨ 核心能力

| 模块 | 说明 |
| --- | --- |
| 📜 **剧本解析** | 自动拆分多集脚本，识别场景、对白、动作描述 |
| 🎨 **分镜生成** | AI 根据剧本文本生成分镜画面，支持批量风格统一 |
| 🎬 **视频合成** | Seedance 2.0 驱动，一键批量生成视频片段 |
| 📝 **字幕对齐** | 自动识别语音生成字幕，精准时间轴对齐 |
| 🎵 **配乐 / 音效** | 场景化配乐推荐与自动拼接 |
| 🔄 **批量化** | 一条命令生成整集，支持断点续跑与失败重试 |

---

## 🛠️ 改良版做了什么

相对原版，本仓库侧重工程稳定性与生产效率：

- **Bug 修复**：修复分镜生成失败、长视频合成中断、字幕时间轴偏移等问题。
- **体验优化**：重构 UI 交互，增加批量预览、进度可视化、错误日志面板。
- **工程化**：完善构建脚本（`scripts/prebuild-cleanup.ps1`），优化打包体积与崩溃恢复。
- **扩展配置**：新增可选的模型 Provider 切换、自定义 Prompt 模板、输出目录策略。

> 详细改动见仓库 CHANGELOG 与 `docs/WORKFLOW_GUIDE.md`。

---

## 🚀 快速开始

```bash
# 安装依赖
npm install

# 开发模式
npm run dev

# 构建 Electron 桌面端
npm run build

# 打包发布
npm run dist
```

---

## 📁 目录结构

```
moyin-manju-improved/
├─ src/               # 主进程 / 渲染进程源码
├─ build/             # 应用图标、资源
├─ scripts/           # 构建与清理脚本
├─ docs/              # 工作流指南、示例剧本
├─ LICENSE
└─ package.json
```

---

## 📜 说明

- **非原创**：本仓库基于公开开源项目进行改良，遵循原项目（AGPL-3.0）许可证。
- **商用合规**：如需商用，请同时遵守上游许可证与所调用 AI 服务的 ToS。
- 改良仅代表对本地工程的维护，不替代原项目官方版本。
