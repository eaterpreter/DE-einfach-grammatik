# Lesson Template（單課輸出結構）

> 共用流程見 **`docs/generation-brief.md`**。練習題型與 `||spoiler||` 見 **`docs/exercise-rules.md`**。全文規範見 **`grammatik-roadmap.md`** §4 起。

---

## 單課檔內不要重複貼的內容

與「例句數量對齊、Practice 分類、Discord spoiler」等相關的**長篇說明**，請只寫在 **`docs/lesson-template.md`** 與 **`docs/exercise-rules.md`**。單課 `.md` 頂多一句話指向 docs。

---

## 粒度與小節（對齊 `grammatik-roadmap.md` §3.0）

- **一 unit 一微主題**：對應 **`docs/build-progress.md` §②** 該列之「**本 unit 微主題**」。勿在同一檔內再塞入 roadmap 已拆成另一列的內容（除非使用者明說合併速通）。
- **何時應拆成獨立 unit**（由規劃端在 roadmap／build-progress 增列，產課端遵守）：**構成 vs 語用**分開、**大對比專章**（如 PII 於完成式 vs 被動）、**圖示／時間軸敘述**獨立成課、**介詞義項群**過多導致單檔例句不足。具體塊狀順序以 **`grammatik-roadmap.md` §3.2** 對應之 **`#### 書 Lxx`** 為準（多書課已有範本）。
- **同檔多小節**（過渡期或主題極短時）：在 **Example Sentences** 內以 **`###` 小節**分組；**每個小節至少 5 句**德語例句（預設與下節一致）。**介詞／格支配**之每一 **義項群** 同此下限（須在小節標題標出義項群；見 roadmap §3.0）。
- **對齊鏈**：每個小節的例句須在 **Sentence Breakdown**、**Common Mistakes** 有**同序、同數**之條目（須逐小節滿足下限；全課總句數可依小節數增加）。

---

生成單一 unit 時，建議依下列 **Markdown 章節** 輸出（標題可視需要微調，但順序與涵蓋內容須對齊 roadmap）。

## Lesson Title

- 標示 Stage、unit 編號（例如 **1-1**、**7-4**）、**書參考 Lx（若有）**與「**本 unit 微主題**」（與 **build-progress** 該列一致）。  
- 檔名須符合 **`docs/generation-brief.md` §5**（`{stage}-{unit}-{slug}.md`）。

## Learning Goal

- 2–4 句（繁中），說明本課學完能做什麼。

## Core Concept

- 本課文法或概念（繁中）：**不要只寫一段口號**。建議 **2～5 個短段**或「先白話、再術語、再提醒易混點」，讓第一次接觸的讀者讀完能說出「這課到底在幹嘛」。  
- 教到 **格（Kasus）** 時，須同時給 **德語名稱 + 通用縮寫**，例如：**Nominativ（主格，Nom.）**、**Akkusativ（賓格，Akk.）**、**Dativ（與格／三格，Dat.）**、**Genitiv（屬格，Gen.）**（依課次取捨），避免只寫「主格／賓格」卻對不到課本與字典。  
- 詳見 **`docs/style-guide.md`** §3「解說深度與口吻」。

## Key Forms / Rules

- 規則、變化表、易混提醒（條列）。

## Example Sentences

- **依本課「小點／句型／義項群」分小節**（`###`），不要混在同一列表而不分類。
- **預設**：每個小節 **至少 5 句**例句（含介詞等工具型義項群；roadmap 或 build-progress 另註者從其註）。一句一行：**`*德語例句*`（中文）**。  
- **疑問句課**（如是非／**W-** 疑問）：例句建議採 **「問句 + 簡短答句」** 成組（仍視為該小節之一「組」；**Breakdown** 可於同一列拆解問、答）。答句用本課已教現在式，順便練 **陳述句語序**。  
- 例句總數須與 **Sentence Breakdown**、**Common Mistakes** 對齊（見下）。

## Sentence Breakdown

- **對齊規則**：與 **Example Sentences** **同序、同句數**。
- 逐句標示：主語／動詞位置／賓語與格／介詞片語等（依句適用）；可用表格或條列。

## Common Mistakes

- **對齊規則**：與 **Example Sentences** **同序、同則數**（原則上每例句對應 1 則常錯示範）。
- 每則建議含：**錯例 → 正例 → 一句話理由**。

## Practice

- **題型與排版**一律依 **`docs/exercise-rules.md`**（四選一、`||spoiler||`、分小節）。
- 單課內 **Practice** 至少分兩類小節；題量見 exercise-rules。
- **不必**另立「Answer Key」大段：答案與解釋放在每題 spoiler 內。

## Quick Review

- 本課 3–5 條重點條列。

---

## 與 roadmap 的對應

- **必提核銷**：產課前對 **`grammatik-roadmap.md` §3.3** 該 **書 L**（見 **build-progress**「書參考」欄）逐條勾選；若一列僅覆蓋該書課之一段，須在 Quick Review 或註記中說明「同書課其餘段見 unit x-y」。
- 若 roadmap 要求多種練習與解析：以 **四選一題型** 滿足，**解析**寫在 `||spoiler||` 內即可。
