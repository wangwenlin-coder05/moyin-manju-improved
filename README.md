# 🎬 Moyin Manju Improved · AI 影视生产工具（改良版）

> **⚠️ 本仓库为第三方改良版，非原创**——系在原项目基础之上进行的二次开发、Bug 修复与功能增强。

<p align="center">
  <a href="https://github.com/wangwenlin333/moyin-manju-improved">
    <img alt="GitHub Stars" src="https://img.shields.io/github/stars/wangwenlin333/moyin-manju-improved?style=for-the-badge&logo=github&logoColor=white&color=181717">
  </a>
  <a href="https://github.com/wangwenlin333/moyin-manju-improved">
    <img alt="GitHub Forks" src="https://img.shields.io/github/forks/wangwenlin333/moyin-manju-improved?style=for-the-badge&logo=github&logoColor=white&color=394867">
  </a>
  <a href="https://github.com/wangwenlin333/moyin-manju-improved/releases">
    <img alt="GitHub Release" src="https://img.shields.io/github/v/release/wangwenlin333/moyin-manju-improved?style=for-the-badge&logo=github&logoColor=white&color=0a66c2">
  </a>
  <a href="https://github.com/wangwenlin333/moyin-manju-improved/releases">
    <img alt="Release 下载" src="https://img.shields.io/github/downloads/wangwenlin333/moyin-manju-improved/total?style=for-the-badge&logo=github&logoColor=white&color=00C4FF">
  </a>
  <a href="https://github.com/wangwenlin333/moyin-manju-improved/issues">
    <img alt="Issues" src="https://img.shields.io/github/issues/wangwenlin333/moyin-manju-improved?style=for-the-badge&logo=github&logoColor=white&color=d73a4a">
  </a>
</p>

<p align="center">
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white">
  <img alt="Electron" src="https://img.shields.io/badge/Electron-28-47848F?style=flat-square&logo=electron&logoColor=white">
  <img alt="AI" src="https://img.shields.io/badge/AI-Video_Chat-D946EF?style=flat-square">
  <img alt="Status" src="https://img.shields.io/badge/Status-改良版-FF6F00?style=flat-square">
  <img alt="License" src="https://img.shields.io/github/license/wangwenlin333/moyin-manju-improved?style=flat-square&color=blue">
</p>

> **AI 影视工业级生产管线**：从剧本到成片的全流程批量化，支持 Seedance 2.0，一键完成分镜生成、视频合成、字幕对齐、配乐选择，极大缩短 AI 短剧 / 漫剧的制作周期。

---

## 🖥️ 下载安装

前往 **Releases** 页面下载桌面安装包（Windows / macOS / Linux）：

[![Download](https://img.shields.io/badge/%F0%9F%93%A6_下载-Release_安装包-00C4FF?style=for-the-badge)](https://github.com/wangwenlin333/moyin-manju-improved/releases)

> 本项目为 Electron 桌面应用，支持本机下载安装；也可 `npm run dev` 本地开发运行。

---

## 📐 处理管线

```mermaid
flowchart LR
    subgraph In["📥 输入"]
        S["剧本 / 脚本 (多集)"]
    end

    subgraph Core["⚙️ AI 生产管线"]
        PA["剧本解析\n分场景 / 对白/动作"]
        PG["分镜生成\nAI 批量画面"]
        PV["视频合成\nSeedance 2.0"]
        SC["字幕对齐\n语音识别"]
        MU["配乐 / 音效\n场景化推荐"]
    end

    subgraph Out["📤 输出"]
        EP["完整剧集成片"]
    end

    S --> PA --> PG --> PV --> SC --> MU --> EP
```

---

## 🛠️ 改良版做了什么

| 类别 | 说明 |
| --- | --- |
| 🐞 Bug 修复 | 修复分镜生成失败、长视频合成中断、字幕时间轴偏移等问题 |
| 🎨 体验优化 | 重构 UI 交互，增加批量预览、进度可视化、错误日志面板 |
| ⚙️ 工程化 | 完善构建脚本，优化打包体积与崩溃恢复 |
| 🔧 扩展配置 | 新增模型 Provider 切换、自定义 Prompt 模板、输出目录策略 |

> 详细改动见仓库 CHANGELOG 与 `docs/WORKFLOW_GUIDE.md`。

---

## 🚀 开发运行

```bash
npm install
npm run dev      # 开发模式
npm run build    # 构建 Electron 桌面端
npm run dist     # 打包发布
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