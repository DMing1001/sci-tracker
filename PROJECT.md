# sci-tracker 项目上下文

## 项目概述
SCI 投稿追踪面板，用于统一管理多篇论文的投稿进度。

## 技术栈
- 纯前端单页应用（HTML + CSS + JS）
- 数据存储：浏览器 localStorage
- 外部 API：Elsevier AuthorHub 公开追踪接口
  - 端点：`https://tnlkuelk67.execute-api.us-east-1.amazonaws.com/tracker/{uuid}`
  - 无需登录，公开访问
  - 从链接 `https://track.authorhub.elsevier.com/?uuid=xxx` 提取 UUID

## 项目路径
`/root/.openclaw/workspace/sci-tracker/`
- `index.html` — 主页面（全部功能在一个文件里）

## 用户需求演进
1. 最初想要一个多投稿进度聚合面板
2. 发现 Elsevier 追踪链接是公开的，可以通过 API 自动获取数据
3. 布局从卡片式 → 表格式 → 条形式，多次迭代
4. 加入中英文切换功能
5. 状态标签用英文，日期、UI 文字支持中英切换

## 设计决策
- 状态标签始终用英文（Under Review / Reviews Complete / Accepted 等），不随语言切换
- 日期格式：中文 `2025年4月6日`，英文 `6 Apr 2025`
- 审稿进展用进度条 + 分数表示（如 1/2）
- 去掉了作者列（第一作者、通讯作者移到展开详情）
- "最近更新时间" 替代了原来的"天数"指标

## GitHub 仓库
- 地址：https://github.com/DMing1001/sci-tracker
- 分支：main
