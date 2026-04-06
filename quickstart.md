# Quickstart（給人看的使用說明）

> 本專案是「德語文法教材 + AI 助教」的檔案結構。  
> 複製下面 **建置期** 或 **讀書期** prompt 到新對話即可。

### 路徑與工作區（請先讀）

- **建議**：將 Cursor **工作區設為 `D:\Notes`**（語言庫根目錄），其下為 **`JP\`**（日文）、**`DE\`**（本專案）。
- 下表 **預設** prompt 使用 **`@D:\Notes\…`** 絕對路徑。
- 若你**只開本 `DE` 資料夾**為工作區，可把 `@D:\Notes\DE\` 改寫成相對根目錄的 **`@docs\…`**、**`@grammatik-roadmap.md`**（建置期 prompt 另含 **`@docs/lesson-template.md`**、**`@docs/style-guide.md`**）。

---

## 這個專案可以怎麼用？

- **作者在補教材**：用「建置期」prompt，依 roadmap 與 `docs/build-progress.md` §② 由小到大產出 `units/`。  
- **學習者在上課**：用「讀書期」prompt，讓 AI 讀 `learner/progress.md` 接續下一課；想用互動情境就選 **B**。  
- **朋友試用**：不必讀完整 docs，貼一段 prompt + 依指示 @ 檔案即可。

---

## 建置期（產教材用）

**工作區 = `D:\Notes`（建議）：**

```text
請持續自動接續（每輪盡量多完成幾個 unit，直到我在對話中喊停；單一對話有長度限制屬正常，可下一則訊息續跑同一策略）：

請讀 @D:\Notes\DE\docs\generation-brief.md（務必含 §3.1）、@D:\Notes\DE\docs\build-progress.md、@D:\Notes\DE\grammatik-roadmap.md、@D:\Notes\DE\docs\lesson-template.md、@D:\Notes\DE\docs\style-guide.md。

依 build-progress §② 由小到大補齊「未產出」列；**優先於同一 Stage 內連續完成**。**勿跳 Stage**（除非我明說跳關）。**僅當該 Stage 在 §② 已無任何「未產出」列時**，才可開始下一 Stage。

每產出或修改 DE\units\（或約定之 DE\reviews\）教材檔，須在同一輪同步更新 DE\docs\build-progress.md §② 對應列（見 generation-brief §4）。產課與修訂須符合 generation-brief §3.1、lesson-template、style-guide 全文（含 Core Concept 深度、格位德語標註、疑問句問答組等）。
```

**工作區 = 僅開 `DE` 資料夾時：**

```text
請持續自動接續（每輪盡量多完成幾個 unit，直到我在對話中喊停；單一對話有長度限制屬正常，可下一則訊息續跑同一策略）：

請讀 @docs/generation-brief.md（務必含 §3.1）、@docs/build-progress.md、@grammatik-roadmap.md、@docs/lesson-template.md、@docs/style-guide.md。

依 build-progress §② 由小到大補齊「未產出」列；**優先於同一 Stage 內連續完成**。**勿跳 Stage**（除非我明說跳關）。**僅當該 Stage 在 §② 已無任何「未產出」列時**，才可開始下一 Stage。

每產出或修改 units/（或約定之 reviews/）教材檔，須在同一輪同步更新 build-progress.md §② 對應列（見 generation-brief §4）。產課與修訂須符合 generation-brief §3.1、lesson-template、style-guide 全文（含 Core Concept 深度、格位德語標註、疑問句問答組等）。
```

---

## 讀書期（用教材學習）

### A. 基本版

**工作區 = `D:\Notes`：**

```text
請讀 @D:\Notes\DE\docs\generation-brief.md 與 @D:\Notes\DE\learner\progress.md，依 progress 接續產出／複習。
```

**工作區 = 僅開 `DE` 資料夾時：**

```text
請讀 @docs/generation-brief.md 與 @learner/progress.md，依 progress 接續產出／複習。
```

### B. 互動教學版（推薦）

**工作區 = 僅開 `DE` 資料夾時：**

```text
請讀 @docs/generation-brief.md 與 @learner/progress.md，依 progress 接續產出／複習。

讀完本課對應的 units/ 或 reviews/ 檔案後，請用「互動教學模式」帶我學，不要只是照抄原文：

- 先用非常短的中文，幫我 recap 本課 2～3 個最核心重點（不用貼原文段落）。
- 之後一小段一小段互動：每次一個重點，先給 1～2 個改寫例句或迷你情境對話，再問我 1 題（選擇或填空），等我回答。
- 題目須嚴格根據本課已教內容，不要超綱。回答後用 1～2 句中文說明對錯。
- 每次出 1 題就停下，除非我說「下一題」。
- 優先生活情境，把本課文法放進小對話裡。

請避免一次貼超過 10 行連續原課文（例句除外），講解以摘要為主。
```

**工作區 = `D:\Notes` 時：** 將上文中的 `@docs/`、`@learner/` 改為 **`@D:\Notes\DE\docs\`**、**`@D:\Notes\DE\learner\`**；讀取教材時路徑為 **`D:\Notes\DE\units\`** 等（其餘句意不變）。
