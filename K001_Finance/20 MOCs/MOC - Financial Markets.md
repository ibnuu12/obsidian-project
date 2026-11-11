---
id: 20260724140000
title: MOC - Financial Markets
aliases:
  - Financial Markets MOC
  - Peta Pasar Keuangan & Perusahaan
tags:
  - zettel/moc
  - financial-markets
created: 2026-07-24 14:00
updated: 2026-07-24 15:35
status: active
type: moc
source: "[[20 MOCs/Master Map of Content]]"
related:
  - "[[20 MOCs/Master Map of Content]]"
  - "[[20 MOCs/MOC - Economics]]"
  - "[[20 MOCs/MOC - Investing]]"
---

# 🏢 MOC - Financial Markets

**Core Purpose**: Domain MOC utama untuk analisis pasar keuangan, pengelompokan sektor industri, strategi rotasi sektoral, serta evaluasi fundamental perusahaan dan *economic moat* emiten.

---

## 🗺️ Knowledge Structure

### 1. 🏬 Sektor Industri & Rotasi Sektoral
* **Taksonomi & Karakteristik Sektor**
  * [[Sector Classification & Rotation Strategies]] — Taksonomi standar empat tingkat pengelompokan sektor industri.
  * [[Sector Classification & Rotation Strategies]] — Karakteristik sektor sensitif siklus makro vs sektor defensif.
* **Rotasi & Strategi Sektoral**
  * [[Sector Classification & Rotation Strategies]] — Taktik penyesuaian alokasi sektor saham mengikuti alur siklus bisnis.

### 2. 🏢 Analisis Fundamental Perusahaan (Company Analysis)
* **Kerangka Riset & Evaluasi Laporan Keuangan**
  * [[Equity Research Analysis Framework]] — Metodologi analisis emiten komprehensif top-down dan bottom-up.
  * [[Financial Statement Analysis]] — Evaluasi kesehatan keuangan, profitabilitas, dan kualitas arus kas.
* **Keunggulan Bersaing & Struktur Modal**
  * [[Competitive Moat Analysis]] — Identifikasi keunggulan kompetitif jangka panjang (*economic moat*).
  * [[Cost of Capital & Corporate Debt Servicing]] — Analisis kemampuan beban utang, solvabilitas, dan biaya modal emiten.

---

## 📌 Dynamic Indexing (Dataview)

```dataview
TABLE type AS Type, status AS Status, file.mtime AS "Last Modified"
FROM #financial-markets OR #sectors OR #companies
WHERE file.name != this.file.name
SORT file.name ASC
```