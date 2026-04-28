# howar31-marketplace

[![Marketplace](https://img.shields.io/badge/Claude%20Code-Marketplace-CC785C?style=for-the-badge)](https://github.com/howar31/howar31-marketplace)
[![License: MIT](https://img.shields.io/github/license/howar31/howar31-marketplace?color=blue&style=for-the-badge)](LICENSE)
[![Sponsor on Ko-fi](https://img.shields.io/badge/sponsor-Ko--fi-FF5E5B?logo=ko-fi&logoColor=white&style=for-the-badge)](https://ko-fi.com/howar31)

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

## 為什麼有 personal marketplace？

- **集中**：之後我發行新 plugin 都掛在這個 marketplace；使用者只要 `marketplace add` 一次，未來新 plugin 自動可見
- **不衝突**：每個 plugin 仍可獨立 self-host（例如 magi-workflow 自己也是個 single-plugin marketplace），給使用者多條安裝路徑選擇

## License

MIT — 見 [LICENSE](LICENSE)。本 marketplace 列出的個別 plugin 各自有獨立 license（見上方各 plugin 連結）。
