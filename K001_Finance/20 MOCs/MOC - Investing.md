---
id: 20260724141500
title: MOC - Investing
aliases:
  - Investing MOC
  - Peta Investasi & Valuasi
tags:
  - zettel/moc
  - investing
created: 2026-07-24 14:15
updated: 2026-07-24 15:35
status: active
type: moc
source: "[[20 MOCs/Master Map of Content]]"
related:
  - "[[20 MOCs/Master Map of Content]]"
  - "[[20 MOCs/MOC - Economics]]"
---

# 💼 MOC - Investing

**Core Purpose**: Domain MOC utama untuk strategi investasi, penentuan nilai intrinsik ekuitas, konstruksi dan diversifikasi portofolio, instrumen pendapatan tetap, serta kerangka pengelolaan risiko modal.

---

## 🗺️ Knowledge Structure

### 1. 📐 Valuasi Ekuitas (Equity Valuation)
* **Intrinsic Valuation (Valuasi Mutlak)**
  * [[Discounted Cash Flow (DCF) Valuation]] — Proyeksi dan diskonto arus kas bebas (*Free Cash Flow*).
  * [[Impact of Rate Hikes on Equity Valuations]] — Analisis kenaikan suku bunga terhadap tingkat diskonto (*Discount Rate* / WACC).
* **Relative Valuation (Valuasi Relatif)**
  * [[Relative Valuation Multiples]] — Pembandingan rasio pasar (P/E, P/BV, EV/EBITDA) terhadap industri.

### 2. 💼 Konstruksi Portofolio & Pendapatan Tetap
* **Teori Portofolio & Alokasi Aset**
  * [[Modern Portfolio Theory (MPT) & Diversification]] — Optimasi risiko dan imbal hasil melalui korelasi aset.
  * [[Capital Asset Pricing Model (CAPM)]] — Pricing aset berbasis risiko sistematis (Beta).
* **Instrumen Penyeimbang & Protection**
  * [[Fixed Income & Corporate Bonds]] — Instrumen obligasi korporasi & pemerintah penyeimbang portofolio.
  * [[Inflation-Hedged Assets]] — Komoditas dan aset riil pelindung nilai portofolio dari erosi inflasi.

### 3. 🛡️ Manajemen Risiko & Perlindungan Modal
* **Pengukuran Risiko Kuantitatif**
  * [[Value at Risk (VaR) & Stress Testing]] — Estimasi potensi kerugian maksimum dan simulasi skenario krisis.
  * [[Yield Curve Dynamics & Recession Indicators]] — Indikator peringatan dini risiko penyesuaian bobot portofolio.
* **Margin keselamatan (Margin of Safety)**
  * [[Probabilistic Thinking & Margin of Safety]] — Batas diskon nilai intrinsik untuk mengantisipasi ketidakpastian.

---

## 📌 Dynamic Indexing (Dataview)

```dataview
TABLE type AS Type, status AS Status, file.mtime AS "Last Modified"
FROM #investing OR #valuation OR #risk-management
WHERE file.name != this.file.name
SORT file.name ASC
```