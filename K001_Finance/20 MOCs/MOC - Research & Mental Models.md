---
id: 20260724142000
title: MOC - Research & Mental Models
aliases:
  - Research & Mental Models MOC
  - Peta Metodologi Riset & Model Mental
tags:
  - zettel/moc
  - mental-models
  - research-workflow
created: 2026-07-24 14:20
updated: 2026-07-24 15:35
status: active
type: moc
source: "[[20 MOCs/Master Map of Content]]"
related:
  - "[[20 MOCs/Master Map of Content]]"
---

# 🛠️ MOC - Research & Mental Models

**Core Purpose**: Domain MOC utama untuk model mental (kerangka pengambilan keputusan rasional), formulasi dan pengujian tesis investasi, serta alur kerja sistematis pengelolaan pengetahuan (*knowledge management workflow*).

---

## 🗺️ Knowledge Structure

### 1. 🧠 Model Mental & Kerangka Keputusan (Mental Models)
* **Strategi Berpikir Kritis**
  * [[Second-Order Thinking]] — Analisis dampak jangka panjang dan efek turunan (*second-order effects*).
  * [[Inversion Principle]] — Pendekatan pemikiran terbalik untuk mengidentifikasi dan menghindari kegagalan.
  * [[Circle of Competence]] — Pengambilan keputusan yang tetap berada di dalam batas area pemahaman riil.
* **Probabilitas & Eksponensial**
  * [[Probabilistic Thinking & Margin of Safety]] — Berpikir berbasis distribusi probabilitas dan marjin keamanan.
  * [[Compounding Effect & Exponential Growth]] — Prinsip efek eksponensial dalam pertumbuhan modal dan ilmu.

### 2. 🎯 Formulasi Tesis Investasi (Investment Thesis)
* **Penyusunan & Rasio Risiko-Hasil**
  * [[Investment Thesis Formulation]] — Kerangka penyusunan tesis hipotesis investasi yang jelas.
  * [[Asymmetric Risk-Reward Tradeoff]] — Pencarian peluang dengan potensi keuntungan jauh melampaui potensi risiko.
* **Pengujian & Exit Strategy**
  * [[Thesis Invalidation Criteria]] — Penetapan kriteria terukur untuk menggugurkan tesis (*exit trigger*).

### 3. 🛠️ Metodologi Riset & Siklus Pengetahuan (Research Workflow)
* **Tangkapan & Pemilahan Informasi**
  * [[Knowledge Management & Research Lifecycle]] — Penangkapan cepat dan alur pemilahan informasi di inbox.
* **Sintesis & Siklus Hidup Pengetahuan**
  * [[Knowledge Management & Research Lifecycle]] — Penyingkatan teks secara bertahap untuk ekstraksi insight.
  * [[Knowledge Management & Research Lifecycle]] — Siklus pengelolaan catatan dari atomik hingga menjadi karya terstruktur.

---

## 📌 Dynamic Indexing (Dataview)

```dataview
TABLE type AS Type, status AS Status, file.mtime AS "Last Modified"
FROM #mental-models OR #research-workflow OR #investment-thesis
WHERE file.name != this.file.name
SORT file.name ASC
```
