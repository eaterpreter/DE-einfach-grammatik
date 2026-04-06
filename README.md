# DE-einfach-grammatik

本 Repo 是**模組化德語文法講義**（繁體中文講解 + 德語例句）：主要給**德語學習者**與自讀者使用。念書時可在 AI 對話中貼上下面 **互動教學版（推薦）** prompt 輔助練習。

## 互動教學版（推薦）

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

**工作區含 `D:\Notes` 時：** 將上文中的 `@docs/`、`@learner/` 改為 `@D:\Notes\DE\docs\`、`@D:\Notes\DE\learner\`；讀取教材時路徑為 `D:\Notes\DE\units\` 等（其餘句意不變）。

- 單元規劃：見根目錄 [`grammatik-roadmap.md`](grammatik-roadmap.md)。
- 學習進度紀錄：見 [`learner/progress.md`](learner/progress.md)（讀書期由 AI 讀此檔接續下一課）。
- 產出進度與單元登錄：見 [`docs/build-progress.md`](docs/build-progress.md) §②（給作者／建置期接手用）。
- 單課範本與題型規格：見 [`docs/lesson-template.md`](docs/lesson-template.md)、[`docs/exercise-rules.md`](docs/exercise-rules.md)、[`docs/style-guide.md`](docs/style-guide.md)。

更完整的使用方式見 [`quickstart.md`](quickstart.md)。

## 單元目錄（TOC）

- [`units/README.md`](units/README.md) — `units/` 目錄說明（檔名規則與模板連結）

### Stage 1

_現在式規則動詞、疑問句、名詞性／格入門、定冠詞變格_

- [動詞現在式（規則變化）入門](units/1-1-present-regular-verbs.md)
- [疑問句語序與類型](units/1-2-questions-word-order.md)
- [性／格與冠詞入門](units/1-3-gender-case-articles-intro.md)
- [定冠詞變格與複數](units/1-4-definite-articles-plural.md)

### Stage 2

_不定冠詞變格、*sein／haben／werden*、動詞位置、複數_

- [不定冠詞變格](units/2-1-indefinite-articles-declension.md)
- [**sein** 現在式人稱變化](units/2-2-sein-present-conjugation.md)
- [**haben** 現在式人稱變化](units/2-3-haben-present-conjugation.md)
- [**werden** 現在式人稱變化](units/2-4-werden-present-conjugation.md)
- [直述句：變位動詞第二位（支點）](units/2-5-verb-position-declarative.md)
- [是非疑問句動詞位置](units/2-6-verb-position-yes-no-questions.md)
- [W-疑問句動詞位置](units/2-7-verb-position-w-questions.md)
- [複數形式與例外](units/2-8-noun-plural-patterns.md)

### Stage 3

_現在式不規則、指示／否定／所有格冠詞、介詞 1–2_

- [不規則動詞現在式](units/3-1-irregular-verbs-present.md)
- [指示冠詞變化](units/3-2-demonstrative-articles.md)
- [**kein** 與 **nicht**（與 *ein* 對照）](units/3-3-kein-nicht-ein.md)
- [所有格冠詞與各格](units/3-4-possessive-articles.md)
- [介詞圖表與內文兩套整理；二格／支配二、三格短語](units/3-5-prepositions-chart-genitive-phrases.md)
- [三格介詞：義項群與例句](units/3-6-dative-prepositions.md)
- [四格介詞](units/3-7-accusative-prepositions.md)
- [可三／四格介詞入門列表](units/3-8-two-way-prepositions-intro.md)
- [Wechselpräpositionen：格義對比](units/3-9-wechsel-prepositions-dat-akku.md)
- [介冠合併（im／ins／zum／am…）](units/3-10-preposition-article-contractions.md)

### Stage 4

_人稱代詞變格、情態與感官動詞、*werden* 未來、*nicht*、可分動詞_

- [人稱代詞變格；**da(r)+介詞**](units/4-1-personal-pronouns-da-prp.md)
- [情態動詞基本（können…wollen）](units/4-2-modal-verbs-basic.md)
- [**möchte** 與禮貌表達](units/4-3-moechte-polite.md)
- [情態動詞否定與單獨使用](units/4-4-modal-negation-standalone.md)
- [**werden** 表未來](units/4-5-werden-future.md)
- [感官動詞 + 原形](units/4-6-perception-verbs-infinitive.md)
- [動詞片語與 **nicht** 的位置（入門）](units/4-7-verb-bracket-nicht.md)
- [可分離與不可分動詞（入門）](units/4-8-separable-prefix-verbs.md)

### Stage 5

_命令式、對等連接詞、從屬連接詞_

- [**du／ihr／Sie** 命令式](units/5-1-imperative-du-ihr-sie.md)
- [**sein／haben／werden** 命令式](units/5-2-imperative-sein-haben-werden.md)
- [可分／不可分與命令式](units/5-3-imperative-separable-verbs.md)
- [語用光譜：請求→命令](units/5-4-imperative-pragmatic-spectrum.md)
- [對等連接詞與從屬入門](units/5-5-coordinating-conjunctions-intro.md)
- [主從句與動詞位置](units/5-6-subordinate-clauses-verb-final.md)
- [*daher／wegen／weil* 與動詞位置](units/5-7-weil-daher-wegen-cause.md)
- [*Trotzdem／Trotz／Obwohl*](units/5-8-trotzdem-trotz-obwohl.md)
- [*wenn* 與位置對調](units/5-9-wenn-condition-word-order.md)
- [*ob* 從句與主句](units/5-10-ob-clause.md)
- [*während／da／wenn* 補充](units/5-11-waehrend-da-wenn-supplement.md)
- [從句整合對比：原因／讓步／條件／是否](units/5-12-subordinate-clauses-integrated-contrast.md)

### Stage 6

_形容詞變格、名詞化、時態總覽、動詞三基本形式_

- [有定冠詞：形容詞變格（弱變化）](units/6-1-adjective-declension-definite-article.md)
- [無冠詞：形容詞變格（強變化）](units/6-2-adjective-declension-no-article.md)
- [不定冠詞與物主冠詞：形容詞變格（混合變化）](units/6-3-adjective-declension-indefinite-article.md)
- [形容詞名詞化](units/6-4-substantivized-adjectives.md)
- [時態系統總覽](units/6-5-tense-system-overview.md)
- [動詞的三種基本形式：原形・過去式・Partizip II](units/6-6-verb-forms-infinitive-prateritum-partizip-ii.md)

### Stage 7

_Präteritum、Perfekt、Plusquamperfekt／Futur II、時態圖、反身_

- [Präteritum：形態與句構](units/7-1-prateritum-morphology-word-order.md)
- [Präteritum：使用情境與語體](units/7-2-prateritum-register-narrative.md)
- [Präteritum：常見動詞與助動詞加強例](units/7-3-prateritum-common-verbs.md)
- [Perfekt：**haben** 與 **sein** 助動詞](units/7-4-perfekt-haben-sein-auxiliary.md)
- [Perfekt：直述與是非疑問語序](units/7-5-perfekt-declarative-yes-no-order.md)
- [Perfekt：**W-** 疑問與從句語序](units/7-6-perfekt-w-questions-subordinate-order.md)
- [Perfekt 與 Präteritum：對照與書列動詞](units/7-7-perfekt-vs-prateritum-verb-choices.md)
- [Perfekt：可分動詞與不可分前綴](units/7-8-perfekt-separable-prefix-verbs.md)
- [Plusquamperfekt：介紹與使用時機](units/7-9-plusquamperfekt-intro-usage.md)
- [Plusquamperfekt：構成與語序](units/7-10-plusquamperfekt-formation.md)
- [Futur II：介紹與使用時機](units/7-11-futur-ii-intro-usage.md)
- [Futur II：構成與語序](units/7-12-futur-ii-formation.md)
- [Perfekt：補充定位與敘事銜接](units/7-13-perfekt-position-linking.md)
- [Perfekt 與多時態對照（敘事銜接）](units/7-14-perfekt-examples-contrast.md)
- [德語時態示意與時間軸敘述](units/7-15-tense-timeline-narrative.md)
- [**sich** 與基本反身用法](units/7-16-reflexive-pronoun-sich-basic.md)
- [反身動詞：**legen／vorstellen** 等](units/7-17-reflexive-verbs-legen-vorstellen.md)
- [三格反身；真反身與假反身](units/7-18-reflexive-dative-true-false.md)
- [相互代詞：**einander** 與 **sich**](units/7-19-reciprocal-pronouns-einander-sich.md)
- [**sich lassen + 原形動詞**](units/7-20-sich-lassen-infinitive.md)

### Stage 8

_被動、*es*、疑問詞、代名詞、關係子句_

- [被動（一）：現在式與過去式 **werden + PII**](units/8-1-passive-present-past-formation.md)
- [被動（二）：完成式與過去完成 **… worden**](units/8-2-passive-perfect-plusquamperfekt.md)
- [被動（三）：直述與疑問的動詞位置](units/8-3-passive-word-order-declarative-questions.md)
- [被動（四）：從句與情態動詞](units/8-4-passive-subordinate-clauses-modals.md)
- [被動（五）：過程 vs 狀態；**man**；**von** 與 **durch**](units/8-5-passive-zustand-man-von.md)
- [**es**：指稱、天氣、時間、距離](units/8-6-es-reference-weather-time-distance.md)
- [*es gibt*／*es handelt sich*／*es dreht sich*](units/8-7-es-gibt-handelt-dreht.md)
- [其他非人稱 **es**](units/8-8-es-impersonal-other.md)
- [**W-** 疑問詞（總覽）](units/8-9-w-interrogatives-overview.md)
- [*was*／*wo* + 介詞縮合：**woran**、**wovon** 等](units/8-10-was-wo-preposition-compounds.md)
- [不定代名詞與指示代名詞](units/8-11-indefinite-demonstrative-pronouns.md)
- [關係代詞：形態與各格](units/8-12-relative-pronouns-forms-cases.md)
- [**Relativsatz**：步驟與英德對照](units/8-13-relativsatz-steps-comparison.md)

### Stage 9

_關係副詞、比較級／*zu*-不定式、分詞_

- [關係副詞；不定關係 **was**／**wer**](units/9-1-relative-adverbs-was-wer-indefinite.md)
- [比較級：謂語、名詞修飾、副詞](units/9-2-comparative-predicate-attributive-adverb.md)
- [最高級：**am …-sten** 與 **der／die／das …-ste**](units/9-3-superlative-am-der-die-das-ste.md)
- [不規則比較級／最高級；**so … wie**；**immer + 比較級**](units/9-4-comparative-irregular-so-wie-immer.md)
- [**je … desto …**（相關比較）](units/9-5-je-desto-comparative-correlative.md)
- [*zu* 不定式：形態與動詞片語](units/9-6-zu-infinitive-formation-phrases.md)
- [*zu* 不定式片語：主／賓／謂補／修飾／介詞結構](units/9-7-zu-infinitive-clause-functions.md)
- [無逗號：**brauchen … zu**、**scheinen zu**、**haben／sein … zu**、**pflegen zu**](units/9-8-zu-infinitive-no-comma-brauchen-scheinen.md)
- [Partizip I：形態與主要用法](units/9-9-partizip-i-forms-uses.md)
- [Partizip II：形態與主要用法](units/9-10-partizip-ii-forms-uses.md)
- [PII：完成式 vs 被動（對比）](units/9-11-partizip-ii-perfekt-vs-passive.md)
- [PII 單獨使用：指示、確認、口語簡答](units/9-12-partizip-ii-standalone-pointing.md)

### Stage 10

_語式、Konjunktiv II／I、引語、數詞_

- [語式與助動詞（入門）](units/10-1-mood-modes-and-auxiliary-verbs.md)
- [Konjunktiv II：假設、直陳與「與事實相反」](units/10-2-konjunktiv-ii-hypothesis-and-fact.md)
- [*würden + Infinitiv*](units/10-3-konjunktiv-ii-wuerden-infinitiv.md)
- [*als ob*／*als wenn* + Konjunktiv II](units/10-4-konjunktiv-ii-als-ob-als-wenn.md)
- [Konjunktiv II：願望、客氣、省略前句](units/10-5-konjunktiv-ii-pragmatics-wishes-polite.md)
- [直接引語](units/10-6-direct-speech-quotes.md)
- [間接引語：連接詞直述（*dass*）](units/10-7-indirect-speech-dass-declarative.md)
- [Konjunktiv I：間接引用](units/10-8-konjunktiv-i-indirect-speech.md)
- [間接引語：易錯與特殊情境](units/10-9-indirect-speech-pitfalls-special.md)
- [數詞：基數、序數、時間、日期](units/10-10-numerals-ordinals-time-date.md)
