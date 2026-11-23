# 知識庫變更日誌 (Changelog)

> 本文件為不可倒退、純追加（append-only）的操作日誌。每次執行文獻入庫 (ingest)、專題查詢 (query) 產出新頁面、或健康度檢查 (lint) 時，LLM 必須在此追加一條記錄。
> 格式規範：`## [YYYY-MM-DD] <操作類型: ingest|query|lint|init> | <標題或說明>`

---

## [2026-11-23] init | 金融證券法規 LLM Wiki 初始化建立

- **操作者**：Antigravity LLM Agent
- **操作說明**：建立知識庫目錄架構 (`raw/papers`, `raw/notes`, `wiki/*`, `assets`)，建立 `index.md` 與 `log.md`，制定 `AGENTS.md` 營運指引。
- **異動檔案**：
  - `AGENTS.md`
  - `index.md`
  - `log.md`


## [2026-11-23] ingest | 2025 證券暨期貨市場執法報告

- **文獻來源**：`raw/papers/2025_FSC_Securities_Futures_Enforcement_Report.pdf`
- **主精讀筆記**：`wiki/papers/2025_證券期貨局_證券暨期貨市場執法報告.md`
- **連動建立/更新實體與法理概念頁面**：
  - `wiki/regulations/證券交易法.md`
  - `wiki/regulations/證券投資人及期貨交易人保護法.md`
  - `wiki/regulations/虛擬資產服務法草案.md`
  - `wiki/concepts/內線交易重大消息明確時點.md`
  - `wiki/concepts/市場操縱與相對成交.md`
  - `wiki/concepts/投保法董監事解任訴訟跨任期與在任要件.md`
  - `wiki/concepts/VASP洗錢防制登記制與業務專法化.md`
  - `wiki/cases/2025_證券期貨重大執法案例彙編.md`
- **目錄更新**：同步更新 `index.md`，登錄 1 篇文獻筆記、3 個法規實體、4 個核心法理、1 個案例彙編。

## [2026-11-23] ingest | 批次入庫 4 篇金融證券法規文獻

- **文獻來源**：
  - `raw/papers/2010_簡兆翌_新修正證券交易法第一百五十七條之一規定簡介.pdf`
  - `raw/papers/2021_投保中心_投資人園地_董監提名與內線交易責任.pdf`
  - `raw/papers/2009_林昌億_證券投資人及期貨交易人保護法最新修正介紹.pdf`
  - `raw/papers/2015_證交所櫃買_鬆綁融資融券限額與風控問答.pdf`
- **精讀筆記產出**：
  - `wiki/papers/2010_簡兆翌_新修正證券交易法第一百五十七條之一規定簡介.md`
  - `wiki/papers/2021_投保中心_投資人園地_董監提名與內線交易責任.md`
  - `wiki/papers/2009_林昌億_證券投資人及期貨交易人保護法最新修正介紹.md`
  - `wiki/papers/2015_證交所櫃買_鬆綁融資融券限額與風控問答.md`
- **法規與概念連動更新**：
  - 更新 `wiki/regulations/證券交易法.md`（增補 §60 信用交易管理與 §157-1 修正史）
  - 更新 `wiki/regulations/證券投資人及期貨交易人保護法.md`（建立 2002～2025 四大演進里程碑，補充 §10-1 與 §35 裁判費立法源頭）
  - 更新 `wiki/concepts/內線交易重大消息明確時點.md`（增列歐盟 MAD/CESR 四大標準與 Basic 案）
  - 新增 `wiki/concepts/信用交易融資融券限額管理與關聯戶控管.md`（關聯戶合併控管與 3 億總歸戶）
  - 新增 `wiki/concepts/董監事候選人提名制與股東權保護.md`（公司法 §192-1、107年修法防弊與假處分救濟）
  - 反向更新 `wiki/papers/2025_證券期貨局_證券暨期貨市場執法報告.md`（串接立法源頭前作）
- **目錄更新**：同步更新 `index.md`。

## [2026-11-23] query | 金融證券法規常見考題解析與互動簡報投影片產出

- **查詢主題**：利用 Wiki 全庫內容，彙整金融證券法規高頻常見考題，產出可獨立播放之 HTML 簡報投影片。
- **產出實體簡報**：`presentations/金融證券法規常見考題_簡報.html`（14 頁互動式投影片，含題型、法條、判準與可折疊擬答）。
- **回寫知識庫綜述**：`wiki/synthesis/金融證券法規常見考題與實務解題綱要.md`。
- **索引更新**：同步登錄至 `index.md` 第 6 節「專題綜述與研究空白」。
