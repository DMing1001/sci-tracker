# SCI Submission Tracker

一站式管理多篇 SCI 论文的投稿进度。

## 功能

- **自动同步**：粘贴 Elsevier 追踪链接，自动获取稿件信息（标题、期刊、审稿状态、审稿人活动）
- **手动管理**：支持非 Elsevier 期刊的手动录入
- **中英切换**：一键切换中文/英文界面
- **筛选排序**：按状态筛选，按任意列排序
- **展开详情**：点击标题查看完整信息（通讯作者、审稿进展、备注）
- **数据导出**：JSON 格式导入/导出，方便备份
- **批量同步**：一键更新所有 Elsevier 投稿的最新状态

## 使用

直接打开 `index.html` 即可，纯前端应用，数据存储在浏览器 localStorage。

## 支持的追踪系统

- Elsevier AuthorHub（自动获取）
- ScholarOne / Editorial Manager 等（手动录入）
