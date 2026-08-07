<div align="center">
  <h1>Klinko AI 市场研究 Skills</h1>
  <p><strong>由 Klinko MCP 驱动的 12 个已完成市场洞察工作流。</strong></p>
  <p>
    <a href="./README.md">🇺🇸 English</a> ·
    <a href="./README.zh-CN.md">🇨🇳 简体中文</a> ·
    <a href="./README.zh-TW.md">🇭🇰 繁體中文</a>
  </p>
  <p>
    <a href="https://klinko.ai/zh/">🌐 Klinko 官网</a> ·
    <a href="https://github.com/klinkoai">🏢 GitHub Organization</a> ·
    <a href="https://home.klinko.ai">🚀 开始市场研究</a>
  </p>
</div>

## 网站预览

### Skills 目录

![面向 Codex 与 Claude Code 的 Klinko AI 市场研究 Skills 目录](./assets/screenshots/skills-hub-zh.jpg)

### Skill 工作流页面

![Klinko 圈层对比器工作流页面](./assets/screenshots/audience-comparator-en.jpg)

## 一套智能能力，十二个清晰工作流

Klinko Skills 把不同的市场问题转化为聚焦、可执行的 Agent 工作流。所有 Skill 共用同一套安全的 Klinko 智能能力，但拥有各自的输入要求、判断流程和输出格式。

| Skill | 能做什么 |
| --- | --- |
| **[Audience Finder](https://github.com/klinkoai/klinko-audience-finder)** | 发现并排序最值得优先服务的目标圈层。 |
| **[Niche Audience Discovery](https://github.com/klinkoai/klinko-niche-audience-discovery)** | 找到容易被忽略的细分人群、新兴圈层和未被满足的社群。 |
| **[Audience Comparator](https://github.com/klinkoai/klinko-audience-comparator)** | 从需求、动机、机会和可触达性比较多个候选圈层。 |
| **[Market Opportunity Analyst](https://github.com/klinkoai/klinko-market-opportunity-analyst)** | 排序市场机会，判断什么最值得优先验证。 |
| **[Startup Idea Validator](https://github.com/klinkoai/klinko-startup-idea-validator)** | 根据用户需求、市场缺口和购买动机验证创业想法。 |
| **[Early Adopter Finder](https://github.com/klinkoai/klinko-early-adopter-finder)** | 找到最可能尝试、采用并主动推荐新产品的人群。 |
| **[Buyer Persona Builder](https://github.com/klinkoai/klinko-buyer-persona-builder)** | 围绕需求、触发因素、顾虑和行为构建买家画像。 |
| **[Customer Pain Point Analyst](https://github.com/klinkoai/klinko-customer-pain-point-analyst)** | 发现反复出现的客户问题，并判断哪些问题正在形成真实需求。 |
| **[Positioning Strategist](https://github.com/klinkoai/klinko-positioning-strategist)** | 把市场缺口和消费者语言转化为更清晰的定位与信息表达。 |
| **[Content Strategy Builder](https://github.com/klinkoai/klinko-content-strategy-builder)** | 根据圈层需求排序内容主题、角度和形式。 |
| **[Creative Brief Generator](https://github.com/klinkoai/klinko-creative-brief-generator)** | 把圈层洞察转化为清晰、可执行的创意简报。 |
| **[Viral Pattern Analyzer](https://github.com/klinkoai/klinko-viral-pattern-analyzer)** | 识别高表现和快速传播内容背后可复用的模式。 |

## 支持平台

- [Codex CLI 与桌面 App](./docs/codex.md) — 已验证
- [Claude Code](./docs/claude-code.md) — 已验证

其他支持 MCP 的客户端需要完成专项验证后，才会列为正式支持平台。

## 目录结构

每个 Skill 已经在 [github.com/klinkoai](https://github.com/klinkoai) 下拥有独立公开仓库和详细工作流页面。公开仓库正在同步已经验证的 MCP 配置与可安装 Skill 包。

程序可以通过 [`catalog.json`](./catalog.json) 读取完整目录。

## 接入状态

12 个工作流和带鉴权的 Klinko MCP 运行层均已完成。当前运行层提供 `match_submit`、`match_get`、`circle_knowledge` 与 `persona_knowledge` 四个工具，并已在 Codex CLI、Codex 桌面 App 与 Claude Code 中验证。公开安装包同步与运行层完成状态分开管理。

## 文档

- [在 Codex 中连接 Klinko MCP](./docs/codex.md)
- [在 Claude Code 中连接 Klinko MCP](./docs/claude-code.md)
- [身份验证](./docs/authentication.md)
- [MCP 运行层概览](./docs/api-overview.md)
- [安全政策](./SECURITY.md)

## 联系我们

[business@klinko.ai](mailto:business@klinko.ai)
