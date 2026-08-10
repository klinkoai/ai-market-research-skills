<div align="center">
  <h1>Klinko AI 市場研究 Skills</h1>
  <p><strong>直接在 Codex 與 Claude Code 中完成目標受眾分析、市場機會發現與驗證。</strong></p>
  <p>
    <a href="./README.md">🇺🇸 English</a> ·
    <a href="./README.zh-CN.md">🇨🇳 简体中文</a> ·
    <a href="./README.zh-TW.md">🇭🇰 繁體中文</a>
  </p>
  <p><a href="#6-個核心市場研究-skills">🌐 瀏覽 Skills</a> · <a href="https://github.com/klinkoai">🏢 GitHub Organization</a> · <a href="https://home.klinko.ai">🚀 開始市場研究</a></p>
</div>

Klinko 是一款 **AI 市場調研工具**，也是一套持續更新的受眾決策引擎，面向創業者、產品團隊、產品行銷與成長團隊。它把公開市場訊號轉化為有優先順序的市場決定：**應該先服務哪類目標受眾、他們需要什麼、市場機會在哪裡，以及下一步驗證什麼**。

## 用一句提示詞安裝

```text
請從 https://github.com/klinkoai/ai-market-research-skills 為目前客戶端安裝 Klinko AI 市場研究 Skills。修改設定前先閱讀倉庫說明，保留現有 Skills 與 MCP 設定，並使用我自己的 API Key 在使用者層級接入帶鑑權的 Klinko MCP。不要讓我把 Key 貼到聊天中，不要顯示或記錄 Key，也不要把 Key 寫入專案或 Git。驗證四個 Klinko 工具，然後說明目前可以使用哪些市場研究 Skills。
```

真實研究需要已授權的 Klinko API Key。手動設定請查看 [Codex 接入文件](./docs/codex.md)、[Claude Code 接入文件](./docs/claude-code.md)與[身分驗證說明](./docs/authentication.md)。

## Klinko 如何進行市場調研

1. 先提出一個有關目標受眾、客戶痛點、市場機會、創業想法、產品定位或內容方向的決策問題。
2. Klinko 透過帶鑑權的 MCP 執行層整理相關公開市場訊號。
3. 對應的 Skill 會在排序前區分證據、解釋、反例與不確定性。
4. 結果以一個可執行的驗證步驟結束，而不是給出缺少證據的市場結論。

## 6 個核心市場研究 Skills

Klinko 將公開目錄聚焦到 6 個邊界清楚、價值最高的市場決策。每個 Skill 都定義專門的輸入、判斷標準、證據邊界、輸出與下一步驗證。

請從目前主倉庫安裝。下面 6 個獨立倉庫是各項能力的公開介紹頁，分別提供決策範例、FAQ 與證據邊界。

| Skill | 支援的決策 | 獨立倉庫 | 詳細說明 |
| --- | --- | --- | --- |
| **受眾發現器** | 應該先服務哪個受眾？ | [GitHub](https://github.com/klinkoai/klinko-audience-finder) | [開啟說明](./references/workflow-audience-finder.md) |
| **客戶痛點分析** | 哪個重複問題正在形成真實需求？ | [GitHub](https://github.com/klinkoai/klinko-customer-pain-point-analyst) | [開啟說明](./references/workflow-customer-pain-point-analyst.md) |
| **市場機會分析** | 哪個市場機會最值得先驗證？ | [GitHub](https://github.com/klinkoai/klinko-market-opportunity-analyst) | [開啟說明](./references/workflow-market-opportunity-analyst.md) |
| **創業想法驗證** | 哪項關鍵假設可能讓想法失敗？ | [GitHub](https://github.com/klinkoai/klinko-startup-idea-validator) | [開啟說明](./references/workflow-startup-idea-validator.md) |
| **定位策略** | 什麼定位與訊息值得測試？ | [GitHub](https://github.com/klinkoai/klinko-positioning-strategist) | [開啟說明](./references/workflow-positioning-strategist.md) |
| **內容策略建構** | 哪些主題、形式與渠道應優先投入？ | [GitHub](https://github.com/klinkoai/klinko-content-strategy-builder) | [開啟說明](./references/workflow-content-strategy-builder.md) |

## 支援客戶端

- [Codex CLI 與桌面 App](./docs/codex.md) — 已驗證
- [Claude Code](./docs/claude-code.md) — 已驗證

## 文件

- [身分驗證](./docs/authentication.md)
- [MCP 執行層概覽](./docs/api-overview.md)
- [機器可讀目錄](./catalog.json)
- [安全政策](./SECURITY.md)

## 研究與信任

- [研究方法](https://klinko.ai/zh/research-methodology/) — 資料來源、證據處理、研究邊界與更新標準
- [關於 Klinko Research](https://klinko.ai/zh/about/) — 發布主體、編輯標準、修正與公司資訊

## 聯絡我們

[business@klinko.ai](mailto:business@klinko.ai)

由 [Klinko](https://github.com/klinkoai) 維護 · 更新於 2026 年 8 月 9 日
