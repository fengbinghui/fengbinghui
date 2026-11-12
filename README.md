<div align="center">

# Hi, I'm Feng Binghui 👋

**AI 应用工程 · Java 后端 · 全栈开发**

把想法落成可交付的产品 —— AI 应用 · 全栈系统 · 内容站点

[![Portfolio](https://img.shields.io/badge/🌐_个人主页-fengbinghui.github.io-0ea5e9?style=for-the-badge)](https://fengbinghui.github.io)
[![Featured](https://img.shields.io/badge/⭐_代表项目-feiyu--ai-6366f1?style=for-the-badge)](https://github.com/fengbinghui/feiyu-ai)
[![New](https://img.shields.io/badge/🆕_2026.11_新作-知阅书库_·_月见小筑-0f9d58?style=for-the-badge)](https://fengbinghui.github.io#work)

</div>

---

## 🧭 关于我

- 🎓 已毕业（人工智能学院），专注 **AI 应用工程** 与 **后端 / 全栈开发**
- 🆕 最近完成两个完整项目：**知阅书库**（Spring Boot + Vue 图书管理全栈系统）与 **月见小筑**（基于 Aurora 二次开发的心月狐主题个人博客）
- 🔭 目前在做：企业级 AI Agent 平台 [**feiyu-ai**](https://github.com/fengbinghui/feiyu-ai) —— 多模型接入、知识库 RAG、MCP 工具、流式对话、文生图 / OCR / Text2SQL
- 🧠 深入方向：**LLM 应用落地**（RAG 召回质量、Agent 工具编排、上下文与成本控制、可观测性、安全边界）
- 🧱 工程习惯：写文档、写测试、做数据库版本化迁移、用 CI 兜底，优先可维护性
- 🎯 目标：做"能上线、可维护、有数据支撑"的产品，而不止步于 Demo

> 我理解的"经验"，不是堆砌技术名词，而是**能把一个复杂系统从跑通、到稳定、到可交付**：知道边界在哪、风险在哪、怎么验证、怎么回滚。

## 🧰 技术栈

**后端**

![Java](https://img.shields.io/badge/Java_17_/_8-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3_/_2.7-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white)
![MyBatis-Plus](https://img.shields.io/badge/MyBatis--Plus-1E90FF?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)
![Flyway](https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white)

**前端**

![Vue](https://img.shields.io/badge/Vue_3_/_2-42b883?style=flat-square&logo=vuedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Pinia](https://img.shields.io/badge/Pinia-FFD859?style=flat-square)
![Element Plus](https://img.shields.io/badge/Element_Plus-409EFF?style=flat-square)
![Element UI](https://img.shields.io/badge/Element_UI-409EFF?style=flat-square)
![ECharts](https://img.shields.io/badge/ECharts-AA344D?style=flat-square)
![Naive UI](https://img.shields.io/badge/Naive_UI-63E2B7?style=flat-square)

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
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)

## 🚀 代表项目

### ⭐ [feiyu-ai](https://github.com/fengbinghui/feiyu-ai) — 企业级 AI Agent 应用平台

> Java 17 · Spring Boot 3.3 · LangChain4j 1.20 · Vue3 / Vben · MySQL 8 · PostgreSQL + pgvector

一个可私有化部署的 AI Agent 平台：管理员接入大模型 → 创建 Agent → 挂载知识库与工具，用户即可流式对话；同时提供文生图、OCR、智能问数、会话分享、操作审计与 Token 用量统计。

- **RAG 工程化**：Tika 解析 → 800/120 滑动窗口切片 → 1024 维向量（qwen-embedding）→ pgvector 检索；向量 + 关键词双通道召回，重索引前清理旧向量避免重复召回
- **流式对话**：后端 WebFlux `Flux<ServerSentEvent>`，前端 `fetch + ReadableStream` 解析；自定义事件协议（delta / rag / tool / completed），过程事件落库可回溯
- **Agent 工具编排**：LangChain4j Tool + 技能包 + MCP（HTTP / STDIO，含 Docker 镜像白名单）；智能问数只允许只读 SQL + 表级授权
- **企业级工程**：RBAC / 登录风控 / BCrypt 平滑迁移 / 敏感字段脱敏 / 上传白名单；AOP 审计异步化 + 90 天清理；11 个资源服务端分页 + DTO 校验；Flyway 接管存量库；28 个单元测试 + Playwright E2E + GitHub Actions CI
- 规模：**13 个 Maven 模块、330 个 Java 文件、30 个 Controller、152 个接口、21 张业务表**

### 📚 知阅书库（ZhiYue Library）— 图书管理全栈系统 · 🔒 私有

> Spring Boot 2.7.8 · MyBatis-Plus 3.5.1 · MySQL 8 · JWT · Knife4j · EasyExcel · Vue 2.6 + Element UI + ECharts

面向校园/社区图书馆的前后端分离系统，覆盖「读者 — 图书管理员 — 系统管理员」三角色的完整借阅业务。

- **借阅业务闭环**：图书 / 分类 / 借阅证 / 借阅规则管理，借书 → 还书 → 逾期查询 → 违章登记 → 借还报表（Excel / PDF 导出），图书支持 EasyExcel 批量导入
- **数据与 AI**：数据总览看板（8 项统计卡片 + 近 4 周借阅量折线 + 借书分类饼图）；AI 智能分析（上传 Excel → 讯飞星火生成 ECharts 配置与分析结论）与读者端 AI 智能推荐（另集成通义千问-Plus，Key 为占位配置、需自备）
- **读者服务**：图书检索与详情、借阅信息、违章查询、读者留言弹幕、公告
- **工程细节**：JWT + 拦截器三角色鉴权（61 个 REST 接口）、Guava RateLimiter 登录限流（2 次/秒）、全局异常统一返回、返回字段脱敏（清除密码等）、WebSocket 实时通道、Knife4j 在线接口文档
- 规模：**152 个 Java 源码文件（含 14 个测试类共 166）、6 个 Controller、61 个接口、14 张表、35 个 Vue 组件**

> 🔒 仓库暂为私有；如需查看源码或演示，欢迎通过 GitHub Issues 联系我。

### 🌙 月见小筑（TSUKIMI LODGE）— 心月狐主题个人博客 · 🔒 私有

> Spring Boot 2.3.7（JDK 8）· MyBatis-Plus · Spring Security + JWT · MySQL 8 · Redis · Vue 3.2 前台 + Vue 2 管理后台

基于开源 [Aurora 博客](https://github.com/linhaojun857/aurora)（Apache-2.0）二次开发的主题化个人博客，把「设计系统」也当作工程来做。

- **双主题设计**：夜月（深色，默认）/ 宣纸（浅色）两套 CSS 变量 token，一键切换并 cookie 记忆；朱砂红 `#C0302B` × 鎏金 `#D9B36A`
- **主题化体验**：心月狐 Hero（月相 / 朱文印章 / 签名）、后台主题设置面板、相册墙、吉祥物三态、主题化 404 与空状态
- **阅读与内容**：Prism 朱砂鎏金代码块、tocbot 目录高亮、顶部阅读进度条、评论审核 + 60 秒频率限制 + 敏感词过滤
- **站点能力**：RSS 2.0 / sitemap / robots、Open Graph、MySQL ngram 全文搜索（可切 Elasticsearch）、邮箱验证码登录（JavaMail 直发）、本地上传 md5 落盘 + 超大图自动压缩
- **工程与文档**：JWT 密钥等配置全部环境变量化、后端 JWT 单测、本地部署说明 / 主题开发说明 / 写作模板 / nginx 示例
- 规模：**101 个 Vue 组件、305 个 Java 文件、21 个 Controller、119 个接口、24 张表**；相对上游基线 **38 次提交、242 个文件变更、+15,978 行**

> 🔒 私有仓库。非官方同人项目，与 KURO GAMES 无关联；角色立绘与素材版权归 KURO GAMES，仅用于个人非商业展示与主题二次创作。

### 🛠 [OISYS](https://github.com/fengbinghui/oisys) — 教务 / 考勤管理系统

> Spring Boot 2.7 · MyBatis-Plus · Spring MVC · Vue2 + Element UI · MySQL

前后端分离的教务与考勤管理：用户 / 角色 / 菜单权限、班级与课程管理、考勤设置与点名记录、登录日志等；含数据库初始化脚本，开箱可跑。

### 🩺 [CommHeatManage](https://github.com/fengbinghui/CommHeatManage) — 社区健康管理系统

> Spring Boot 3.1 · Spring Security + JWT · MyBatis-Plus · Vue3 + Element Plus + ECharts

社区健康档案与数据管理：账号与权限、健康报告、数据归档与统计图表；前后端分离，附 API 接口文档与压测脚本。

### 🌱 学习与实验

- [Spring-MVC_for_learn](https://github.com/fengbinghui/Spring-MVC_for_learn) — 手写 SpringMVC 核心机制：前端控制器、视图解析、注解映射
- [springcloud-config](https://github.com/fengbinghui/springcloud-config) — Spring Cloud Config 配置中心的多环境配置实践

## 🖼 界面预览

<p align="center">
  <img src="https://fengbinghui.github.io/assets/img/yuejian-home.jpg" width="49%" alt="月见小筑 · 心月狐主题首页" />
  <img src="https://fengbinghui.github.io/assets/img/zhiyue-dashboard.png" width="49%" alt="知阅书库 · 数据总览" />
</p>

## 📊 我如何做工程

| 维度 | 我的做法 | 证据 |
| --- | --- | --- |
| **架构** | 模块化单体，依赖单向（server → 领域 → 公共），按能力拆分边界 | feiyu-ai 13 个 Maven 模块 |
| **安全** | 认证 / 授权 / 风控 / 脱敏 / 上传白名单 / 错误码收敛，逐项验证边界 | 401 / 403 / 429 / 400 验收脚本；知阅书库 JWT + 限流 |
| **数据** | 数据库版本化（Flyway），存量库 baseline 接管，迁移前备份 + 临时库演练 | V1 基线 + V2 审计增强 |
| **质量** | 单测 + 接口验收 + 真实浏览器 E2E + 类型检查 + CI | 28 单测 / E2E 15 项 / typecheck 0 错误 |
| **可观测** | 操作审计 + 模型调用统计（Token / 耗时 / 成功率 / 配额） | 审计日志页 / 用量分析页 |
| **AI 工程** | 检索质量（TopK / 阈值 / 双通道）、上下文成本（记忆窗口）、工具安全（只读 SQL / 白名单） | feiyu-ai RAG / Agent 功能 |
| **设计系统** | 先定 design token（配色 / 字体 / 间距 / 圆角），再做组件与状态；换肤只改 token，不动结构 | 月见小筑双主题（夜月 / 宣纸） |

## 🗓 编程轨迹

```
2022  ┌─ 注册 GitHub，开始系统学习编程
2023  ├─ SpringMVC / SpringCloud 学习实践，后端基础与全栈项目起步
2024  ├─ 大量阅读优秀开源后端 / 前端项目（Vue 生态、权限与低代码框架）
2025  ├─ 社区健康管理系统（前后端分离 / Spring Security + JWT / ECharts）
2026  ├─ 完成毕业设计与教务考勤系统（OISYS）
      ├─ 毕业，转向 AI 应用工程方向
      ├─ 企业级 AI Agent 平台 feiyu-ai：RAG / Agent / MCP / 工程化落地
      ├─ 知阅书库：Spring Boot + Vue 全栈图书管理系统
      └─ 月见小筑：Aurora 二次开发的心月狐主题个人博客 ← 现在
```

## 📈 语言分布

<div align="center">

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=fengbinghui&layout=compact&langs_count=8&theme=github_dark&hide_border=true&bg_color=0D1117)

</div>

## 🤝 交流

- 个人主页：**[fengbinghui.github.io](https://fengbinghui.github.io)**
- 代表项目：**[feiyu-ai](https://github.com/fengbinghui/feiyu-ai)**
- 欢迎通过 **GitHub Issues / Discussions** 交流 AI 应用工程、后端架构与全栈实践
- 知阅书库、月见小筑为私有项目，如需查看源码或交流实现细节，欢迎联系我

<div align="center">

**Keep building. 把复杂留给设计，把简单留给用户。**

</div>
