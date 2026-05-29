<h1 align="center">MateClaw</h1>

<p align="center">企业 AI 数字员工系统 —— 让 AI 真正融入你的工作流</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.1.5-blue" />
  <img src="https://img.shields.io/badge/platform-macOS%20%7C%20Windows%20%7C%20Linux-lightgrey" />
  <img src="https://img.shields.io/badge/electron-40-47848F?logo=electron" />
  <img src="https://img.shields.io/badge/react-19-61DAFB?logo=react" />
  <img src="https://img.shields.io/badge/typescript-5.8-3178C6?logo=typescript" />
</p>

---

## 产品定位

MateClaw 是一套面向企业的 **AI 数字员工平台**。不同于普通 AI 助手，MateClaw 中的每个数字员工都拥有独立的角色身份、记忆系统、技能库和企业工具接入能力，能够真正替代人工完成钉钉审批跟进、飞书文档整理、邮件归类回复、数据库查询分析、浏览网页、定时自动化任务等重复性工作。

**核心理念：AI 不只是聊天框，而是一位真正上岗的数字同事。**

---

## 亮点功能

### 多模型自由切换，国内外全覆盖

内置 13+ 主流 LLM 提供商，一键切换，无需反复配置 API：

| 国际 | 国内 |
|------|------|
| Claude 4 (Opus / Sonnet / Haiku) | DeepSeek V4 Pro / Flash |
| GPT-5.5 / GPT-4.1 / o3 / o4-mini | 通义千问 Qwen3-max / plus |
| Gemini 3 Pro / 2.5 Flash | Kimi K2.5 / K2 Thinking |
| OpenRouter 聚合 | 智谱 GLM-5 / GLM-4.7、MiniMax M2.5 |

### 企业渠道全面接入

数字员工可以直接在企业应用里"上班"，而不是待在一个独立的聊天窗口里：

- **钉钉** — 企业消息、审批流、自动化（WebSocket 流式连接）
- **飞书 / Lark** — 消息、文档、权限卡片交互
- **企业微信** — 组织消息、流式回复
- **邮件** — IMAP/SMTP，支持 Gmail、Outlook、QQ 邮箱、网易等
- **Telegram / WhatsApp / QQ** — 个人渠道接入

### 强大的企业连接器

数字员工可以读懂和操作企业里真实的数据与系统：

- **数据库** — MySQL、PostgreSQL、SQLite、SQL Server（只读安全模式）
- **代码仓库** — GitHub（Issue、PR、Actions 读取）
- **对象存储** — AWS S3、MinIO、阿里云 OSS
- **SSH** — 远程主机指令执行
- **邮箱** — 多账户统一管理

### 技能系统 + 800+ 现成技能

员工技能热加载，安装即用，支持自定义开发。内置技能涵盖：

- 浏览器自动化（支持 Shadow DOM、复杂 SPA）
- PDF / Excel / Word 文档处理
- 网页内容提取与搜索
- AI 绘图
- 兼容Codex 插件系统

### 记忆 + 定时任务 + 子智能体

- **持久记忆**：员工跨会话记住上下文，无需每次重复说明背景
- **定时任务**：Cron 调度，员工可在指定时间自动执行任务
- **子智能体**：员工可以拆解复杂任务，调度其他员工协作完成

### 浏览器自动化

内置浏览器操控能力，支持需要登录的网站、动态页面、Shadow DOM，可用于淘宝/小红书/B站/亚马逊等数据采集、RPA 替代、网页操作自动化。

---

## 技术栈

| 层次 | 技术 |
|------|------|
| 桌面框架 | Electron 40 |
| 前端 | React 19 + TypeScript 5.8 + Vite 6 |
| 样式 | Tailwind CSS 4 + shadcn/ui |
| 状态管理 | Zustand + Immer |
| 本地数据库 | SQLite (better-sqlite3) 
| 日志 | Winston + Winston Daily Rotate |

---

## 支持平台

| 平台 | 架构 | 安装包格式 |
|------|------|-----------|
| macOS | x64 / Apple Silicon (ARM64) | DMG、ZIP |
| Windows | x64 | NSIS 安装程序 |
| Linux | x64 | AppImage |
