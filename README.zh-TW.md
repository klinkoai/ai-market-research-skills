<div align="center">
  <h1>Klinko AI 市場研究 Skills</h1>
  <p><strong>由 Klinko MCP 驅動的 12 個已完成市場洞察工作流程。</strong></p>
  <p>
    <a href="./README.md">🇺🇸 English</a> ·
    <a href="./README.zh-CN.md">🇨🇳 简体中文</a> ·
    <a href="./README.zh-TW.md">🇭🇰 繁體中文</a>
  </p>
  <p>
    <a href="https://klinko.ai/zh/">🌐 Klinko 官網</a> ·
    <a href="https://github.com/klinkoai">🏢 GitHub Organization</a> ·
    <a href="https://home.klinko.ai">🚀 開始市場研究</a>
  </p>
</div>

## 用一句提示詞安裝

把下面這段提示詞直接複製到 Codex 或 Claude Code。Agent 會讀取本倉庫，依照你正在使用的客戶端完成使用者層級設定並驗證連線。

```text
請從 https://github.com/klinkoai/ai-market-research-skills 為目前的客戶端安裝並設定 Klinko AI 市場研究 Skills。開始操作前，先閱讀倉庫 README，以及與目前客戶端對應的 Codex 或 Claude Code 接入文件。請使用使用者層級設定接入帶鑑權的 Klinko MCP，保留我現有的 MCP 設定，並驗證 match_submit、match_get、circle_knowledge 和 persona_knowledge 四個工具均可用。不要顯示、記錄、提交 API Key，也不要把 Key 寫進任何專案檔案。如果需要 Key，請先指導我將它儲存在本機 ~/.klinko_mcp_qa_key，並把檔案權限設為 600；等我確認後再繼續。完成後請準確說明修改了哪些設定以及驗證結果。
```

安裝需要已授權的 Klinko MCP API Key。不要把 Key 貼到提示詞中，也不要提交到 Git。手動設定可查看 [Codex 接入文件](./docs/codex.md)、[Claude Code 接入文件](./docs/claude-code.md)和[身分驗證說明](./docs/authentication.md)。

## 網站預覽

### Skills 目錄

![面向 Codex 與 Claude Code 的 Klinko AI 市場研究 Skills 目錄](./assets/screenshots/skills-hub-en.jpg)

### Skill 工作流程頁面

![Klinko Audience Comparator 工作流程頁面](./assets/screenshots/audience-comparator-en.jpg)

## 一套智慧能力，十二個清晰工作流程

Klinko Skills 把不同的市場問題轉化為聚焦、可執行的 Agent 工作流程。所有 Skill 共用同一套安全的 Klinko 智慧能力，但擁有各自的輸入要求、判斷流程和輸出格式。

| Skill | 能做什麼 |
| --- | --- |
| **[Audience Finder](https://github.com/klinkoai/klinko-audience-finder)** | 發現並排序最值得優先服務的目標圈層。 |
| **[Niche Audience Discovery](https://github.com/klinkoai/klinko-niche-audience-discovery)** | 找到容易被忽略的細分受眾、新興圈層和未被滿足的社群。 |
| **[Audience Comparator](https://github.com/klinkoai/klinko-audience-comparator)** | 從需求、動機、機會和可觸達性比較多個候選圈層。 |
| **[Market Opportunity Analyst](https://github.com/klinkoai/klinko-market-opportunity-analyst)** | 排序市場機會，判斷什麼最值得優先驗證。 |
| **[Startup Idea Validator](https://github.com/klinkoai/klinko-startup-idea-validator)** | 根據使用者需求、市場缺口和購買動機驗證創業想法。 |
| **[Early Adopter Finder](https://github.com/klinkoai/klinko-early-adopter-finder)** | 找到最可能嘗試、採用並主動推薦新產品的受眾。 |
| **[Buyer Persona Builder](https://github.com/klinkoai/klinko-buyer-persona-builder)** | 圍繞需求、觸發因素、顧慮和行為建立買家人物誌。 |
| **[Customer Pain Point Analyst](https://github.com/klinkoai/klinko-customer-pain-point-analyst)** | 發現反覆出現的客戶問題，並判斷哪些問題正在形成真實需求。 |
| **[Positioning Strategist](https://github.com/klinkoai/klinko-positioning-strategist)** | 把市場缺口和消費者語言轉化為更清晰的定位與訊息表達。 |
| **[Content Strategy Builder](https://github.com/klinkoai/klinko-content-strategy-builder)** | 根據圈層需求排序內容主題、角度和形式。 |
| **[Creative Brief Generator](https://github.com/klinkoai/klinko-creative-brief-generator)** | 把圈層洞察轉化為清晰、可執行的創意簡報。 |
| **[Viral Pattern Analyzer](https://github.com/klinkoai/klinko-viral-pattern-analyzer)** | 識別高表現和快速傳播內容背後可重複使用的模式。 |

## 支援平台

- [Codex CLI 與桌面 App](./docs/codex.md) — 已驗證
- [Claude Code](./docs/claude-code.md) — 已驗證

其他支援 MCP 的客戶端需要完成專項驗證後，才會列為正式支援平台。

## 目錄結構

每個 Skill 已經在 [github.com/klinkoai](https://github.com/klinkoai) 下擁有獨立公開倉庫和詳細工作流程頁面。公開倉庫正在同步已驗證的 MCP 設定與可安裝 Skill 套件。

程式可以透過 [`catalog.json`](./catalog.json) 讀取完整目錄。

## 接入狀態

12 個工作流程和帶鑑權的 Klinko MCP 執行層均已完成。目前執行層提供 `match_submit`、`match_get`、`circle_knowledge` 與 `persona_knowledge` 四個工具，並已在 Codex CLI、Codex 桌面 App 與 Claude Code 中驗證。公開安裝套件同步與執行層完成狀態分開管理。

## 文件

- [在 Codex 中連接 Klinko MCP](./docs/codex.md)
- [在 Claude Code 中連接 Klinko MCP](./docs/claude-code.md)
- [身分驗證](./docs/authentication.md)
- [MCP 執行層概覽](./docs/api-overview.md)
- [安全政策](./SECURITY.md)

## 聯絡我們

[business@klinko.ai](mailto:business@klinko.ai)
