---
license: cc-by-4.0
language:
  - en
  - pl
pretty_name: "Ballpoints.org — Iconic Ballpoint Pens Encyclopedia, 7-Criteria Legend Evaluations & Refill Standards (EN/PL)"
description: "Bilingual (EN/PL) encyclopedia dataset of 28 iconic ballpoint, rollerball, and gel pens, 224 evidence-backed evaluations across a 7-criteria industrial design rubric, 32 refill standards and cartridges (ISO 12757-2 / Parker G2, D1, Euro-style), and 12 historic stationery manufacturers from Ballpoints.org."
size_categories:
  - n<1K
task_categories:
  - text-classification
  - question-answering
  - tabular-classification
tags:
  - industrial-design
  - stationery
  - ballpoint-pens
  - design-history
  - product-taxonomy
  - iso-standards
  - museum-collections
  - bilingual
---

# Ballpoints.org — Iconic Ballpoint Pens Encyclopedia, 7-Criteria Legend Evaluations & Refill Standards (EN/PL)

> **Canonical Web Encyclopedia (EN):** [https://ballpoints.org/en/](https://ballpoints.org/en/)  
> **Kanoniczna Encyklopedia (PL):** [https://ballpoints.org/pl/](https://ballpoints.org/pl/)  
> **Refill Standards & Dimensions Guide:** [https://ballpoints.org/en/refills/](https://ballpoints.org/en/refills/) | [https://ballpoints.org/pl/wklady/](https://ballpoints.org/pl/wklady/)  
> **7-Criteria Rubric & Methodology:** [https://ballpoints.org/en/methodology/](https://ballpoints.org/en/methodology/) | [https://ballpoints.org/pl/metodologia/](https://ballpoints.org/pl/metodologia/)

---

## English Overview

**[Ballpoints.org](https://ballpoints.org/en/)** (*Ikoniczne Długopisy*) is a bilingual (English & Polish) reference encyclopedia and industrial design research dataset dedicated to iconic ballpoint pens, rollerballs, gel pens, and pressurized/hybrid non-fountain writing instruments.

Unlike commercial stationery catalogs, **Ballpoints.org** evaluates every candidate model against a strict, source-verified **7-Criteria Legend Rubric**, explicitly recording both **positive and negative findings** and distinguishing between **model-specific evidence** (`applies_to: "model"` or `"variant"`, which count towards the score) and **line- or brand-level halo effects** (`applies_to: "line"` or `"brand"`, recorded as context only). A model enters the catalogue with at least 2 of 7 criteria met:

1. **`longevity`** — Uninterrupted decades of production with documented continuity of the specific model.
2. **`design-recognition`** — Permanent museum collection holdings (e.g., [MoMA Architecture and Design](https://ballpoints.org/en/pens/bic-cristal/), Centre Pompidou, Cooper Hewitt) or major industrial design awards (Good Design, Red Dot, iF) with inventory numbers and acquisition provenance.
3. **`technical-first`** — Documented origination of a mechanism, ink chemistry, or dimensional standard that reshaped the writing instrument industry.
4. **`cultural-footprint`** — Documented role outside stationery (spaceflight hardware, state treaty signings, lexicographical genericization in major dictionaries, or fine art).
5. **`scale`** — Verified cumulative production scale in the hundreds of millions or billions of units.
6. **`enthusiast-canon`** — Sustained critical consensus across independent stationery publications (*The Pen Addict*, *The Gentleman Stationer*, *JetPens*, etc.).
7. **`user-practice`** — Documented occupational, institutional, or subcultural adoption (e.g., military issue, architectural drafting, pen spinning, aviation).

### Dataset Contents

| File (JSON & CSV pairs) | Records | Description |
| :--- | :---: | :--- |
| `iconic-ballpoint-pens-catalog.json` / `.csv` | **28** | Complete physical, historical, and technical profiles of 28 iconic writing instruments (e.g., [BIC Cristal](https://ballpoints.org/en/pens/bic-cristal/), [Parker Jotter](https://ballpoints.org/en/pens/parker-jotter/), [Lamy 2000 Ballpoint](https://ballpoints.org/en/pens/lamy-2000-ballpoint/), [Fisher Space Pen AG7](https://ballpoints.org/en/pens/fisher-space-pen-ag7/), [Caran d'Ache 849](https://ballpoints.org/en/pens/caran-dache-849/), [Pilot Hi-Tec-C](https://ballpoints.org/en/pens/pilot-hi-tec-c/), [uni Jetstream](https://ballpoints.org/en/pens/uni-jetstream/), [Ball Pentel R50](https://ballpoints.org/en/pens/pentel-ball-pentel-r50/), [Pilot Precise V5](https://ballpoints.org/en/pens/pilot-precise-v5/)). `legend_criteria_met_model_count` is the published score (model- and variant-scope criteria met). |
| `seven-criteria-legend-evaluations.json` / `.csv` | **224** | Granular evidence records across the 7-criteria rubric (including both `met: true` and documented `met: false` refutations) in English and Polish with primary source citations. |
| `ballpoint-refill-standards-and-dimensions.json` / `.csv` | **32** | Technical and dimensional specifications (`length_mm`, `diameter_mm`, `iso_standard`) for 32 refill standards and cartridges ([Parker-style G2 / ISO G2](https://ballpoints.org/en/refills/#parker-g2), [D1 multipen](https://ballpoints.org/en/refills/#d1), Euro-style rollerball, Schmidt P900/EasyFlow, Fisher PR, Lamy M16, Caran d'Ache Goliath, etc.). |
| `stationery-brands-catalog.json` / `.csv` | **12** | Historical profiles of 12 writing instrument manufacturers ([BIC](https://ballpoints.org/en/brands/bic/), [Parker](https://ballpoints.org/en/brands/parker/), [Lamy](https://ballpoints.org/en/brands/lamy/), [Caran d'Ache](https://ballpoints.org/en/brands/caran-dache/), [Pilot](https://ballpoints.org/en/brands/pilot/), [Uni / Mitsubishi Pencil](https://ballpoints.org/en/brands/uni/), [Zebra](https://ballpoints.org/en/brands/zebra/), [Pentel](https://ballpoints.org/en/brands/pentel/), [Monami](https://ballpoints.org/en/brands/monami/), etc.). |

---

## Opis po polsku (Polish Overview)

**[Ballpoints.org — Ikoniczne Długopisy](https://ballpoints.org/pl/)** to dwujęzyczna (polsko-angielska) encyklopedia wzornictwa przemysłowego poświęcona ikonicznym długopisom kulkowym, żelowym, rollerom i długopisom ciśnieniowym.

Każdy z **28 modeli** w katalogu jest weryfikowany według jawnej, siedmiokryterialnej rubryki dowodowej ([Metodologia i kryteria oceny](https://ballpoints.org/pl/metodologia/)), która oddziela fakty dotyczące konkretnego modelu długopisu od ogólnej renomy marki lub wersji pióra wiecznego (np. w przypadku [Lamy 2000](https://ballpoints.org/pl/dlugopisy/lamy-2000-ballpoint/) czy [Ball Pentel R50](https://ballpoints.org/pl/dlugopisy/pentel-ball-pentel-r50/)). Zbiór zawiera również ustrukturyzowany przewodnik wymiarowy po **32 standardach wkładów** ([Przewodnik po wkładach](https://ballpoints.org/pl/wklady/)).

---

## Citation & License

Released under **Creative Commons Attribution 4.0 International (CC BY 4.0)**. When using this dataset in research, design history studies, RAG systems, or stationery compatibility tools, please attribute **Ballpoints.org** with a canonical link:

```bibtex
@misc{pytlarz2026ballpoints,
  author       = {Pytlarz, Piotr},
  title        = {Ballpoints.org: Iconic Ballpoint Pens Encyclopedia, 7-Criteria Legend Evaluations and Refill Standards (EN/PL)},
  year         = {2026},
  url          = {https://ballpoints.org/},
  note         = {CC BY 4.0 Open Data Package}
}
```
