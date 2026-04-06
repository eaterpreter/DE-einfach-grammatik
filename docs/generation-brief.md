# Generation Brief（AI 生成教材：固定入口）

> 本檔為 **多對話共用** 的流程與分工。詳盡教學內容與必教清單以專案根目錄 **`grammatik-roadmap.md`** 為準；與本檔若有落差，以 roadmap 為優先。

### 路徑與工作區

- **建議**將 Cursor 工作區設為 **`D:\Notes`**（語言庫根；見 **`D:\Notes\README.md`**），德語專案路徑為 **`D:\Notes\DE\`**。
- 於 prompt 中引用檔案時，建議使用 **`@D:\Notes\DE\docs\generation-brief.md`**、**`@D:\Notes\DE\grammatik-roadmap.md`** 等（與 **`quickstart.md`** 一致）。
- 若工作區**只開本 `DE` 資料夾**，可仍用相對 **`@docs/…`**、**`@grammatik-roadmap.md`**。

---

## 1. 新對話要 @ 誰（固定 prompt）

僅需複製兩行時，見專案根目錄 **`quickstart.md`**（與本節文字一致；若更動 prompt 請兩處同步）。

### 建置期（產出／補齊 `units/`）

建議一次 @ 三檔（**第三檔決定教學邊界，不可省略**）：

`@docs/generation-brief.md`、`@docs/build-progress.md`、**`@grammatik-roadmap.md`**（工作區為 **`D:\Notes` 時建議：** **`@D:\Notes\DE\docs\generation-brief.md`**、**`@D:\Notes\DE\docs\build-progress.md`**、**`@D:\Notes\DE\grammatik-roadmap.md`**）

接續建置時：依 **build-progress** §② 與下節 **「Stage 順序」**；每產出或修改 `units/`（或約定之 `reviews/`）教材檔，須在同一輪同步更新 **build-progress.md §②** 對應列（見 **§4**）。

（若只貼兩檔，也請**務必**另開或同輪讀取 **`grammatik-roadmap.md`** 對照當前 Stage／§2 必教，避免內容漂移。）

### 穩定讀書期（產出／複習教材）

請讀 `@docs/generation-brief.md` 與 `@learner/progress.md`，依 **progress** 接續產出／複習。

---

## 2. 讀檔順序與 Stage 順序（建議）

1. **`grammatik-roadmap.md`**：對照當前 **Stage**（**§3.1** 總覽）、**粒度原則**（**§3.0**）、**拆段範本**（**§3.2**，含 **L11–L39** 等多個 `#### 書 Lxx`）、必覆蓋（§2）、**書上必提核銷**（**§3.3**）、輸出類型（§4 起）。**教學內容邊界以此檔為準**，不得與前後 unit 矛盾（除非 roadmap 已改並註明）。
2. **`docs/build-progress.md`**：**建置期**「下一格該產哪一個 unit」；**§② 未產出列**為準。
3. **Stage 順序（建置期）**：除非使用者明確要求跳關，否則 **同一 Stage 內依 unit 序號由小到大補齊**，**勿**在 **Stage N 仍有未產出列時**逕自產出 **Stage N+1**。
4. **讀書期**：`learner/progress.md`（若狀態為「已啟用」）。
5. **產出單一 unit 時**：`docs/lesson-template.md`、`docs/exercise-rules.md`、`docs/style-guide.md`（見下節分工）。

---

## 3. 檔案分工（避免重複定義）

| 檔案 | 負責 |
|------|------|
| `grammatik-roadmap.md` | 學什麼、順序、必教；**§3.0** 粒度；**§3.1** Stage 總覽；**§3.2** 重課拆段（**多書課**範本）；**§3.3** 書 Lektion 必提核銷與建議 unit |
| `docs/lesson-template.md` | 單課 **章節結構**；例句／Breakdown／Mistakes 對齊等 |
| **`docs/exercise-rules.md`** | **題型名稱**、四選一、`||spoiler||`、題量 |
| `docs/style-guide.md` | 繁中語氣、德語例句風格、錯誤提醒口吻 |

**單課細節**：以 **`lesson-template.md`** + **`exercise-rules.md`** 為準；`generation-brief.md` 不重複列條款。

### 3.1 全專案產課／修訂 `units/` 的最低標準（強制）

凡 **新增、改寫、回補** `units/`（含 **已標「已有」** 的檔案），皆須符合：

- **`docs/style-guide.md`**：**§3.1**（**Core Concept** 解說深度與口吻）、**§3.2**（格位 **德語全名 + 縮寫**，如 **Nominativ（Nom.）**）、**§1.1**（台灣繁中用語）。  
- **`docs/lesson-template.md`**：**Core Concept** 不可只剩口號段；**Example Sentences** 每 **`###`** 下限、**疑問句課**之 **問答組** 例句、**Breakdown／Mistakes** 對齊鏈等。

**目的**：避免「只有某幾課特別好懂、其餘照舊很硬」的版本分裂。**Stage 2 以後未產出之 unit** 一律適用；**Stage 1 已產出**者若規格升級，應分批回補至同一標準。

---

## 4. 強制：`docs/build-progress.md` 必須隨產出更新（接手用）

**`build-progress.md` 是本專案「現在做到哪一格」的唯一進度表**。下列情況 **在同一輪對話／同一次提交內** 必須改好 `build-progress.md`，**不可**只產檔不更新表：

1. **新增或完成** `units/`（或約定之 `reviews/`）內任一教材檔 → 在 **§② 教材產出追蹤** 對應 **Stage／unit 列** 填入**完整檔名**（須符合 **§5 檔名慣例**），狀態改為 **已有**。若 roadmap 增列新 unit，須先在 **§② 插入新列**（並同步 **`grammatik-roadmap.md` §3.3** 之「建議 unit」）。
2. **刪除、更名、作廢**某 unit 檔 → 同步修正該列或註明作廢。
3. **更動 brief／lesson-template／exercise-rules／style-guide** 且影響後續產出 → 視需要更新 **§① 規格管線** 或於 **build-progress**「修訂備註」註記。
4. **大幅修訂**某個已標「已有」之 unit 檔 → 建議於 **build-progress**「修訂備註」簡述日期與要點。

若做不到同步更新，應在結尾明確列出「請下一則訊息更新 `build-progress.md`：…」。**漏更新等於打斷接手鏈**。

---

## 5. 單元編號與 `units/` 檔名（全專案一致）

### 5.1 單元編號

- 格式：**`stage-unit`**（兩段非負整數），例如 **`1-1`**、**`7-4`**。第二段 **`unit`** 為該 Stage 內**遞增序號**，**可大於 4**（見 **`grammatik-roadmap.md` §3.0**）。
- **書本 Lektion**：**不**再以單一公式強制對應；**書參考**、**微主題** 以 **`docs/build-progress.md` §②** 為準，**必提核銷** 以 **`grammatik-roadmap.md` §3.3** 為準。一書課可對 **多列** unit。

### 5.2 教材檔檔名（強制慣例）

- **型樣**：**`{stage}-{unit}-{slug}.md`**
- **`{slug}`**：**英文小寫 kebab-case**，簡短描述主題，**不含空格、中文、全形標點**。
- 例：`1-1-present-regular-verbs.md`

---

## 6. `learner/progress.md` 與 `learner/error-log.md`

- **建置期**：兩檔可先存在，狀態為 **尚未啟用**。
- **啟用時機**：**第一份 `units/` 教材產出，且學習者確認要開始用教材學習時**，再將 `progress.md` 改為啟用。

---

## 7. 監督步（可選）

完成初稿後，可要求：對照 `grammatik-roadmap.md` 當前 Stage 與本檔 checklist，檢查漏項與超綱例句，再修改檔案。
