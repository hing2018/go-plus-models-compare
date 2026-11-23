# OpenCode Go Plus 模型對比儀表板

互動式單頁網頁，比較 OpenCode Go Plus（$40/月）方案中各模型的：

- 月限額（官方 models API）
- input 單價 / 1M
- $40 可買 token 量
- 真正成本 / 1M（含實測 allowance 倍率）
- 額度倍數
- 上文數量（context window）
- 編碼能力 / 智力（定性分級）
- 速度（本機 streaming 實測 t/s）
- 實測倍率（折扣 / 加價）

## 資料來源

- `https://opencode.ai/inference/go/v1/models`（2026-11-23 抓取）
- 本機實測 `usage.opencode.{list_cost, allowance, billing_source}`（streaming 200 output tokens）

所有數據為 2026-11-23 快照，方案額度與折扣可能隨時變動。

## 使用

直接開啟 `index.html`，或造訪 GitHub Pages。

功能：欄位排序、關鍵字搜尋、依智力/編碼/倍率篩選、一鍵隱藏未能測速或使用的模型。
