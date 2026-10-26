# 智能体工场（Cursor Plugin）

连接 [智能体工场](https://agent.bitilinks.cn)：项目 / 任务 MCP + Agent 技能（含代签 PAT 流程）。

## 包含

- **Logo**：`assets/logo.svg`（品牌三叶标）
- **Skill**：`skills/agent-factory`（连工场、列项目、建任务 demo）
- **MCP**：`mcp.json` → `https://agent.bitilinks.cn/api/connector/mcp`
- **变量**：`AF_CONNECTOR_TOKEN`（Bearer `afpat_…`，在 Plugins → Configure 填写；勿贴到聊天）

## 本地试用

1. 复制本目录到 `~/.cursor/plugins/local/agent-factory`
2. Cursor 里 Reload Window
3. Customize 确认插件与技能；Configure 填入 PAT（或由 bot 按技能代签后写入）

## 发布

- 推到公开 GitHub 仓库后，提交 [Marketplace](https://cursor.com/marketplace/publish)
- 或 Teams：Dashboard → Plugins & MCPs → 导入仓库到团队市场

## 鉴权约定

禁止用户手抄 PAT 到聊天。优先账密登录 → `POST /api/connector/tokens` 签发 → 写入连接器 / 插件变量。
