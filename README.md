# howar31-marketplace

[![Marketplace](https://img.shields.io/badge/Claude%20Code-Marketplace-CC785C?style=for-the-badge)](https://github.com/howar31/howar31-marketplace)
[![License: MIT](https://img.shields.io/github/license/howar31/howar31-marketplace?color=blue&style=for-the-badge)](LICENSE)
[![Sponsor](https://img.shields.io/badge/Sponsor-donate.howar31.com-b4532c?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI+PHBhdGggZmlsbD0iI2ZmZiIgZD0iTTIwLjg0IDQuNjFhNS41IDUuNSAwIDAgMC03Ljc4IDBMMTIgNS42N2wtMS4wNi0xLjA2YTUuNSA1LjUgMCAwIDAtNy43OCA3Ljc4bDEuMDYgMS4wNkwxMiAyMS4yM2w3Ljc4LTcuNzggMS4wNi0xLjA2YTUuNSA1LjUgMCAwIDAgMC03Ljc4eiIvPjwvc3ZnPg==)](https://donate.howar31.com/)

> Howar31 個人的 Claude Code plugin marketplace。集中管理我所有公開發行的 plugins。

## 安裝 marketplace

註冊本 marketplace 一次即可，之後所有 plugin 都從這裡安裝：

```bash
claude plugin marketplace add howar31/howar31-marketplace
```

或在 Claude Code session 裡用 slash command：

```
/plugin marketplace add howar31/howar31-marketplace
```

## 可用 plugins

### 🧠 magi-workflow

多模型協作的軟體工程 workflow plugin。Plan / Tasks / Implementation / Code review / Commit 全流程串接，含智慧型 dispatcher 路由、MAGI 加權投票審議、契約 drift 自動偵測。

- **Source**: [howar31/magi-workflow](https://github.com/howar31/magi-workflow)
- **License**: MIT
- **安裝**：

```bash
claude plugin install magi@howar31
```

完整功能說明見 [magi-workflow README](https://github.com/howar31/magi-workflow#readme)。

### 🧠 mem（claude-memory）

跨 cwd 記憶的 read / write skills，補強 Claude Code 內建 auto-memory：`/mem:recall` 跨所有專案目錄搜尋記憶、`/mem:memorize` 稽核當前對話並寫入。純檔案系統，無 vector DB、無 MCP。

- **Source**: [howar31/claude-memory](https://github.com/howar31/claude-memory)
- **License**: MIT
- **安裝**：

```bash
claude plugin install mem@howar31
```

完整功能說明見 [claude-memory README](https://github.com/howar31/claude-memory#readme)。

### 🌐 browser（browser-automation）

操作真實（headless）瀏覽器，做 curl / HTTP 腳本做不到的事：點擊／輸入、截圖與 PDF、網路攔截／mock／觀察、CDP 層級除錯、跨瀏覽器 E2E（Puppeteer + Playwright）。model-invoked，依任務自動觸發。

- **Source**: [howar31/browser-automation](https://github.com/howar31/browser-automation)
- **License**: MIT
- **安裝**：

```bash
claude plugin install browser@howar31
```

完整功能說明見 [browser-automation README](https://github.com/howar31/browser-automation#readme)。

### 🤝 handoff

把當前 session 存成 LLM-facing 的交接文件，讓下一個 agent（即使是不同模型、空白 context）能冷啟動接手：任務目標、現況、決策（含理由與被否決方案）、死路、硬限制、待解問題、下一步。`/handoff` 存檔、`/handoff load` 接續；model-invoked，也吃「做交接」「接續交接」等自然語句。

- **Source**: [howar31/handoff](https://github.com/howar31/handoff)
- **License**: MIT
- **安裝**：

```bash
claude plugin install handoff@howar31
```

完整功能說明見 [handoff README](https://github.com/howar31/handoff#readme)。

## 為什麼有 personal marketplace？

- **集中**：之後我發行新 plugin 都掛在這個 marketplace；使用者只要 `marketplace add` 一次，未來新 plugin 自動可見
- **不衝突**：每個 plugin 仍可獨立 self-host（例如 magi-workflow 自己也是個 single-plugin marketplace），給使用者多條安裝路徑選擇

## License

MIT — 見 [LICENSE](LICENSE)。本 marketplace 列出的個別 plugin 各自有獨立 license（見上方各 plugin 連結）。
