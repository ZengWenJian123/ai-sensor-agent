# Development 计划草案（占位）

## 技术建议（MVP）
- 前端：React / Next.js
- 后端：Node.js + NestJS（或 FastAPI）
- 数据库：PostgreSQL
- 检索：PostgreSQL 全文检索（早期）

## 模块拆分
1. quote-service（语录读取/检索）
2. people-service（人物信息）
3. admin-service（录入与审核）

## 开发节奏
- Sprint 1：数据模型 + 基础 API
- Sprint 2：核心页面 + 搜索
- Sprint 3：审核后台 + 上线准备

## 工程规范
- 提交前运行 lint + test
- 文档与接口同步更新
- 所有语录记录需带来源字段
