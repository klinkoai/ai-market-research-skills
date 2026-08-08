<div align="center">
  <h1>Klinko AI 市场研究 Skills</h1>
  <p><strong>6 个核心 Skills，覆盖圈层研究、市场验证、定位与内容决策。</strong></p>
  <p>
    <a href="./README.md">🇺🇸 English</a> ·
    <a href="./README.zh-CN.md">🇨🇳 简体中文</a> ·
    <a href="./README.zh-TW.md">🇭🇰 繁體中文</a>
  </p>
  <p>
    <a href="#6-个核心市场研究-skills">🌐 浏览核心 Skills</a> ·
    <a href="https://github.com/klinkoai">🏢 GitHub Organization</a> ·
    <a href="https://home.klinko.ai">🚀 开始市场研究</a>
  </p>
</div>

## 用一句提示词安装

把下面这段提示词复制到 Codex 或 Claude Code：

```text
请从 https://github.com/klinkoai/ai-market-research-skills 为当前客户端安装 Klinko AI 市场研究 Skills。修改配置前先阅读仓库说明，保留我已有的 Skills 和 MCP 配置，并使用我自己的 API Key 在用户级接入带鉴权的 Klinko MCP。不要让我把 Key 发到聊天里，不要显示或记录 Key，也不要把 Key 写入项目或 Git。验证 match_submit、match_get、circle_knowledge 和 persona_knowledge 四个工具，然后说明完成了哪些配置以及目前可以使用哪些市场研究 Skills。
```

真实研究需要已授权的 Klinko API Key。手动配置请查看 [Codex 接入文档](./docs/codex.md)、[Claude Code 接入文档](./docs/claude-code.md)和[身份验证说明](./docs/authentication.md)。

## 网站预览

![Klinko 的 6 个核心 AI 市场研究 Skills](./assets/screenshots/skills-hub-zh.jpg)

![圈层对比 AI 市场研究 Skill](./assets/screenshots/audience-comparator-en.jpg)

## 6 个核心市场研究 Skills

Klinko 将公开目录聚焦到 6 个边界清晰、价值最高的市场决策。每个 Skill 都定义了专门的输入、判断标准、证据边界、输出和下一步验证。

| Skill | 支持的决策 |
| --- | --- |
| [圈层发现器](./references/workflow-audience-finder.md) | 应该先研究哪个圈层？ |
| [客户痛点分析](./references/workflow-customer-pain-point-analyst.md) | 哪个重复问题正在形成真实需求？ |
| [市场机会分析](./references/workflow-market-opportunity-analyst.md) | 哪个市场机会最值得先验证？ |
| [创业想法验证](./references/workflow-startup-idea-validator.md) | 哪项关键假设可能让想法失败？ |
| [定位策略](./references/workflow-positioning-strategist.md) | 什么定位和信息值得测试？ |
| [内容策略构建](./references/workflow-content-strategy-builder.md) | 哪些主题、形式和渠道应优先投入？ |

这 6 个核心 Skills 从圈层发现一路覆盖到市场行动，避免把相近搜索意图拆成过多公开选项。安装包仍保留需要时可调用的其他研究操作。

## 安装包结构

```text
ai-market-research-skills/
├── SKILL.md                     # 入口与通用执行规则
├── agents/openai.yaml           # 面向用户的 Skill 定义
├── references/
│   ├── mcp-setup.md
│   ├── mcp-tools.md
│   └── workflow-*.md            # 专门的研究说明
└── docs/                        # 客户端接入和安全文档
```

## 支持客户端

- [Codex CLI 与桌面 App](./docs/codex.md) — 已验证
- [Claude Code](./docs/claude-code.md) — 已验证

MCP 运行层提供 `match_submit`、`match_get`、`circle_knowledge` 和 `persona_knowledge`。6 个核心 Skills 与鉴权运行层均已完成。

## 文档

- [在 Codex 中连接 Klinko MCP](./docs/codex.md)
- [在 Claude Code 中连接 Klinko MCP](./docs/claude-code.md)
- [身份验证](./docs/authentication.md)
- [MCP 运行层概览](./docs/api-overview.md)
- [机器可读目录](./catalog.json)
- [安全政策](./SECURITY.md)

## 联系我们

[business@klinko.ai](mailto:business@klinko.ai)
