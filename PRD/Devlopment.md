# Development 计划（v0.2）

## 1. 技术方向（MVP）
- 前端：Next.js + Tailwind CSS
- 后端：FastAPI（优先快速落地）
- 数据库：PostgreSQL（本地可用 Docker 启动）
- 检索：PostgreSQL ILIKE/全文检索（早期）

## 2. MVP 功能模块
1. quote-service：语录查询、随机推荐、搜索。
2. submission-service：用户投稿、状态流转。
3. review-service：审核通过/驳回。
4. taxonomy-service：人物、标签维护。

## 3. 鉴权策略（按你要求）
- 当前阶段不做登录/注册。
- 管理端可先用本地环境变量口令或内网访问方式临时保护。
- 后续再升级正式权限系统。

## 4. 运行与测试
- 优先支持本地运行（前后端 + DB）。
- 目标命令（建议）：
  - `docker compose up -d db`
  - `pnpm dev`（前端）
  - `uvicorn app.main:app --reload`（后端）

## 5. Sprint 建议
- Sprint 1：数据模型 + API 草版 + 首页/UI 基础。
- Sprint 2：人物页、搜索页、投稿页联通。
- Sprint 3：审核流程、稳定性优化、本地联调。

## 6. 交付标准
- 所有语录必须有最小来源字段。
- 投稿必须经过审核后可见。
- 前端样式统一使用 Tailwind CSS。
