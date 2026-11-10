<div align="center">

# Hi, I'm Feng Binghui 👋

**AI 应用工程 · Java 后端 · 全栈开发**

把 LLM 能力落成可交付的产品 —— RAG · Agent · MCP · 流式对话 · 工程化

[![Portfolio](https://img.shields.io/badge/🌐_个人主页-fengbinghui.github.io-0ea5e9?style=for-the-badge)](https://fengbinghui.github.io)
[![Featured](https://img.shields.io/badge/⭐_代表项目-feiyu--ai-6366f1?style=for-the-badge)](https://github.com/fengbinghui/feiyu-ai)

</div>

---

## 🧭 关于我

- 🎓 人工智能学院在读，长期专注 **AI 应用工程** 与 **后端 / 全栈开发**
- 🔭 目前在做：企业级 AI Agent 平台 [**feiyu-ai**](https://github.com/fengbinghui/feiyu-ai) —— 多模型接入、知识库 RAG、MCP 工具、流式对话、文生图 / OCR / Text2SQL
- 🧠 深入方向：**LLM 应用落地**（RAG 召回质量、Agent 工具编排、上下文与成本控制、可观测性、安全边界）
- 🧱 工程习惯：写文档、写测试、做数据库版本化迁移、用 CI 兜底，优先可维护性
- 🎯 目标：做"能上线、可维护、有数据支撑"的 AI 应用，而不止步于 Demo

> 我理解的"经验"，不是堆砌技术名词，而是**能把一个复杂系统从跑通、到稳定、到可交付**：知道边界在哪、风险在哪、怎么验证、怎么回滚。

## 🧰 技术栈

**后端**

![Java](https://img.shields.io/badge/Java_17-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![MyBatis-Plus](https://img.shields.io/badge/MyBatis--Plus-1E90FF?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white)

**前端**

![Vue](https://img.shields.io/badge/Vue_3-42b883?style=flat-square&logo=vuedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Pinia](https://img.shields.io/badge/Pinia-FFD859?style=flat-square)
![Naive UI](https://img.shields.io/badge/Naive_UI-63E2B7?style=flat-square)
![Element Plus](https://img.shields.io/badge/Element_Plus-409EFF?style=flat-square)

**AI / LLM**

![LangChain4j](https://img.shields.io/badge/LangChain4j-1.20-6B46C1?style=flat-square)
![RAG](https://img.shields.io/badge/RAG-检索增强生成-0ea5e9?style=flat-square)
![MCP](https://img.shields.io/badge/MCP-模型上下文协议-8b5cf6?style=flat-square)
![SSE](https://img.shields.io/badge/SSE-流式输出-10b981?style=flat-square)
![pgvector](https://img.shields.io/badge/pgvector-向量检索-336791?style=flat-square&logo=postgresql&logoColor=white)

**工具与平台**

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white)
![pnpm](https://img.shields.io/badge/pnpm-F69220?style=flat-square&logo=pnpm&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=flat-square&logo=playwright&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)

## 🚀 代表项目

### ⭐ [feiyu-ai](https://github.com/fengbinghui/feiyu-ai) — 企业级 AI Agent 应用平台

> Java 17 · Spring Boot 3.3 · LangChain4j 1.20 · Vue3 / Vben · MySQL 8 · PostgreSQL + pgvector

一个可私有化部署的 AI Agent 平台：管理员接入大模型 → 创建 Agent → 挂载知识库与工具，用户即可流式对话；同时提供文生图、OCR、智能问数、会话分享、操作审计与 Token 用量统计。

- **RAG 工程化**：Tika 解析 → 800/120 滑动窗口切片 → 1024 维向量（qwen-embedding）→ pgvector 检索；向量 + 关键词双通道召回，重索引前清理旧向量避免重复召回
- **流式对话**：后端 WebFlux `Flux<ServerSentEvent>`，前端 `fetch + ReadableStream` 解析；自定义事件协议（delta / rag / tool / completed），过程事件落库可回溯
- **Agent 工具编排**：LangChain4j Tool + 技能包 + MCP（HTTP / STDIO，含 Docker 镜像白名单）；智能问数只允许只读 SQL + 表级授权
- **企业级工程**：RBAC / 登录风控 / BCrypt 平滑迁移 / 敏感字段脱敏 / 上传白名单；AOP 审计异步化 + 90 天清理；11 个资源服务端分页 + DTO 校验；Flyway 接管存量库；28 个单元测试 + Playwright E2E + GitHub Actions CI
- 规模：**13 个 Maven 模块、330 个 Java 文件、30 个 Controller、152 个接口、21 张业务表**

### 🛠 [OISYS](https://github.com/fengbinghui/oisys) — 教务 / 考勤管理系统

> Spring Boot 2.7 · MyBatis-Plus · Spring MVC · Vue2 + Element UI · MySQL

前后端分离的教务与考勤管理：用户 / 角色 / 菜单权限、班级与课程管理、考勤设置与点名记录、登录日志等；含数据库初始化脚本，开箱可跑。

### 🩺 [CommHeatManage](https://github.com/fengbinghui/CommHeatManage) — 社区健康管理系统

> Spring Boot 3.1 · Spring Security + JWT · MyBatis-Plus · Vue3 + Element Plus + ECharts

社区健康档案与数据管理：账号与权限、健康报告、数据归档与统计图表；前后端分离，附 API 接口文档与压测脚本。

### 🌱 学习与实验

- [Spring-MVC_for_learn](https://github.com/fengbinghui/Spring-MVC_for_learn) — 手写 SpringMVC 核心机制：前端控制器、视图解析、注解映射
- [springcloud-config](https://github.com/fengbinghui/springcloud-config) — Spring Cloud Config 配置中心的多环境配置实践

## 📊 我如何做工程

| 维度 | 我的做法 | 证据 |
| --- | --- | --- |
| **架构** | 模块化单体，依赖单向（server → 领域 → 公共），按能力拆分边界 | feiyu-ai 13 个 Maven 模块 |
| **安全** | 认证 / 授权 / 风控 / 脱敏 / 上传白名单 / 错误码收敛，逐项验证边界 | 401 / 403 / 429 / 400 验收脚本 |
| **数据** | 数据库版本化（Flyway），存量库 baseline 接管，迁移前备份 + 临时库演练 | V1 基线 + V2 审计增强 |
| **质量** | 单测 + 接口验收 + 真实浏览器 E2E + 类型检查 + CI | 28 单测 / E2E 15 项 / typecheck 0 错误 |
| **可观测** | 操作审计 + 模型调用统计（Token / 耗时 / 成功率 / 配额） | 审计日志页 / 用量分析页 |
| **AI 工程** | 检索质量（TopK / 阈值 / 双通道）、上下文成本（记忆窗口）、工具安全（只读 SQL / 白名单） | feiyu-ai RAG / Agent 功能 |

## 🗓 编程轨迹

```
2022  ┌─ 注册 GitHub，开始系统学习编程
2023  ├─ SpringMVC / SpringCloud 学习实践，后端基础与全栈项目起步
2024  ├─ 大量阅读优秀开源后端 / 前端项目（Vue 生态、权限与低代码框架）
2025  ├─ 社区健康管理系统（前后端分离 / Spring Security + JWT / ECharts）
2026  ├─ 教务考勤系统（OISYS）、毕业设计
      └─ 企业级 AI Agent 平台 feiyu-ai：RAG / Agent / MCP / 工程化落地 ← 现在
```

## 📈 语言分布

<div align="center">

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=fengbinghui&layout=compact&langs_count=8&theme=github_dark&hide_border=true&bg_color=0D1117)

</div>

## 🤝 交流

- 个人主页：**[fengbinghui.github.io](https://fengbinghui.github.io)**
- 代表项目：**[feiyu-ai](https://github.com/fengbinghui/feiyu-ai)**
- 欢迎通过 **GitHub Issues / Discussions** 交流 AI 应用工程、后端架构与全栈实践

<div align="center">

**Keep building. 把复杂留给设计，把简单留给用户。**

</div>
