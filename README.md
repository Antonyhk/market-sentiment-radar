# Market Sentiment Radar

> **A research toolkit for tracking public narratives and sentiment shifts around businesses.**
>
> Sentiment is a prompt for further research—not a substitute for fundamentals, valuation, or independent judgment.

## Purpose

`market-sentiment-radar` provides a transparent structure for observing how public narratives evolve around a company, sector, or identifiable event. Its purpose is to turn dispersed public discussion into **testable research questions** that can be checked against primary disclosures, operating metrics, and a pre-existing investment thesis.

This project deliberately separates source types and documents its assumptions. It does not combine heterogeneous sources into a single opaque score, generate buy/sell signals, or infer private information.

## Research workflow

```text
Observe public narratives
        ↓
Label source type, event, and sentiment
        ↓
Identify the narrative shift
        ↓
Form a testable question
        ↓
Verify against primary evidence and business fundamentals
        ↓
Record confirming or disconfirming evidence
```

## Repository structure

| Path | Contents |
|---|---|
| [`methodology/`](methodology/) | Source policy, classification guide, and limitations. |
| [`data/`](data/) | A clearly labelled hypothetical sample dataset and field definitions. |
| [`reports/`](reports/) | Example event-window research write-ups. |
| `templates/` | Reusable narrative-review template. |

## Included sample

The sample dataset is **hypothetical** and exists only to demonstrate a transparent research workflow. It does not describe a real company, market event, or investment conclusion.

## Core principles

1. **Fundamentals first.** Public sentiment can guide research attention but cannot establish business quality or intrinsic value.
2. **Source separation.** Company disclosures, professional media, public social discussion, and search interest are different inputs and remain separately labelled.
3. **Event context.** Observations must be connected to an identifiable event window rather than presented as timeless sentiment.
4. **Falsifiability.** Every material narrative should lead to an observable question and a stated condition that could disconfirm it.
5. **Auditability.** Records should preserve source URLs, dates, evidence excerpts, analyst notes, and a confidence label.

## Minimum observation schema

| Field | Description |
|---|---|
| `timestamp` | Observation date and time in ISO 8601 format. |
| `source_type` | Controlled category, such as `company_disclosure`, `professional_media`, `public_social`, or `search_trend`. |
| `company_or_topic` | Company, sector, or research topic being observed. |
| `event_tag` | Identifiable event or time-window label. |
| `narrative_label` | Concise statement of the public narrative being tracked. |
| `sentiment_label` | `positive`, `neutral`, `negative`, or `mixed`. |
| `evidence_excerpt` | Short source-grounded observation; do not store personal or non-public data. |
| `analyst_note` | The research question or verification step created by the observation. |
| `confidence` | `high`, `medium`, or `low`, reflecting evidence clarity and coverage—not a price forecast. |

## Boundaries

This repository is for research documentation and educational purposes. Do not use it to publish personal data, non-public information, platform content obtained contrary to its terms, or automated trading instructions.

## Status

**Stage:** Research framework and illustrative sample data.  
**Next step:** Expand the examples only after confirming data licensing, source terms, and reproducible methodology.

## Disclaimer

This repository is for research and educational purposes only. It does not constitute investment, legal, tax, or financial advice.
