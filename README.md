# Market Sentiment Radar｜市場情緒雷達

> **A research toolkit for tracking public narratives and sentiment shifts around businesses.**  
> **用於追蹤企業相關公共敘事與情緒變化的研究工具。**
>
> Sentiment is a prompt for further research—not a substitute for fundamentals, valuation, or independent judgment.  
> 情緒是進一步研究的提示，而非基本面、估值或獨立判斷的替代品。

## Purpose｜目的

`market-sentiment-radar` provides a transparent structure for observing how public narratives evolve around a company, sector, or identifiable event. Its purpose is to turn dispersed public discussion into **testable research questions** that can be checked against primary disclosures, operating metrics, and a pre-existing investment thesis.

`market-sentiment-radar` 提供一套透明架構，用於觀察公司、產業或可辨識事件周邊的公共敘事如何演變。其目的在於將零散的公開討論轉化為**可驗證的研究問題**，並以一手披露、營運指標及既有投資論點作核對。

This project separates source types and documents its assumptions. It does not combine heterogeneous sources into a single opaque score, generate buy/sell signals, or infer private information.

本專案會分開標記來源類型並記錄假設，不會將異質來源混合為單一不透明分數、產生買賣訊號，或推斷非公開資訊。

## Research Workflow｜研究流程

```text
Observe public narratives｜觀察公共敘事
        ↓
Label source type, event, and sentiment｜標記來源類型、事件與情緒
        ↓
Identify the narrative shift｜辨識敘事變化
        ↓
Form a testable question｜建立可驗證問題
        ↓
Verify against primary evidence and fundamentals｜以一手證據與基本面驗證
        ↓
Record confirming or disconfirming evidence｜記錄支持或反證
```

## Repository Structure｜儲存庫結構

| Path｜路徑 | Contents｜內容 |
|---|---|
| [`methodology/`](methodology/) | Source policy, classification guide, and limitations. ／ 來源政策、分類指引與限制。 |
| [`data/`](data/) | Clearly labelled hypothetical sample data and field definitions. ／ 清楚標示為假設性的範例資料與欄位定義。 |
| [`reports/`](reports/) | Example event-window research write-ups. ／ 事件窗口研究撰寫範例。 |
| [`templates/`](templates/) | Reusable narrative-review template. ／ 可重複使用的敘事檢閱範本。 |

## Included Sample｜範例資料

The sample dataset is **hypothetical** and exists only to demonstrate a transparent research workflow. It does not describe a real company, market event, or investment conclusion.

範例資料集為**假設性內容**，僅用於示範透明的研究流程；它並不描述真實公司、市場事件或投資結論。

## Core Principles｜核心原則

| Principle｜原則 | English | 中文 |
|---|---|---|
| Fundamentals first｜基本面優先 | Public sentiment can guide research attention but cannot establish business quality or intrinsic value. | 公共情緒可引導研究注意力，但不能證明企業品質或內在價值。 |
| Source separation｜來源分離 | Company disclosures, professional media, public social discussion, and search interest remain separately labelled. | 公司披露、專業媒體、公開社交討論與搜尋關注度必須分開標記。 |
| Event context｜事件脈絡 | Observations must be tied to an identifiable event window. | 每項觀察必須連結至可辨識的事件窗口。 |
| Falsifiability｜可證偽性 | Material narratives should lead to an observable question and a disconfirming condition. | 重要敘事應引出可觀察的問題及反證條件。 |
| Auditability｜可稽核性 | Preserve source URLs, dates, excerpts, notes, and confidence labels. | 保留來源網址、日期、摘錄、筆記與信心標籤。 |

## Minimum Observation Schema｜最低觀察欄位

| Field｜欄位 | Description｜說明 |
|---|---|
| `timestamp` | Observation date and time in ISO 8601 format. ／ ISO 8601 格式的觀察日期與時間。 |
| `source_type` | Controlled source category. ／ 受控的來源類型。 |
| `company_or_topic` | Company, sector, or research topic. ／ 公司、產業或研究主題。 |
| `event_tag` | Identifiable event or time-window label. ／ 可辨識的事件或時間窗口標籤。 |
| `narrative_label` | Concise public narrative being tracked. ／ 正在追蹤的簡潔公共敘事。 |
| `sentiment_label` | `positive`, `neutral`, `negative`, or `mixed`. ／ `positive`、`neutral`、`negative` 或 `mixed`。 |
| `evidence_excerpt` | Short, source-grounded observation. ／ 基於來源的簡短觀察。 |
| `analyst_note` | Research question or verification step created by the observation. ／ 由觀察產生的研究問題或驗證步驟。 |
| `confidence` | Evidence clarity and coverage, not a price forecast. ／ 證據清晰度與覆蓋度，而非價格預測。 |

## Boundaries｜使用界線

This repository is for research documentation and educational purposes. Do not use it to publish personal data, non-public information, platform content obtained contrary to its terms, or automated trading instructions.

本儲存庫僅用於研究記錄與教育用途。請勿用於發布個人資料、非公開資訊、違反平台條款取得的內容或自動交易指令。

## Status｜狀態

**Stage｜階段：** Research framework and illustrative sample data. ／ 研究框架與示範性範例資料。  
**Next step｜下一步：** Expand examples only after confirming data licensing, source terms, and reproducible methodology. ／ 僅在確認資料授權、來源條款與可重現方法後才擴充範例。

## Disclaimer｜免責聲明

This repository is for research and educational purposes only. It does not constitute investment, legal, tax, or financial advice.

本儲存庫僅供研究與教育用途，不構成投資、法律、稅務或財務建議。
