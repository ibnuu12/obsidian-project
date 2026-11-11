---
id: 20260724135000
title: MOC - Economics
aliases:
  - Economics MOC
  - Peta Ekonomi Makro
tags:
  - zettel/moc
  - economics
created: 2026-07-24 13:50
updated: 2026-07-24 15:35
status: active
type: moc
source: "[[20 MOCs/Master Map of Content]]"
related:
  - "[[20 MOCs/Master Map of Content]]"
---

# 🏛️ MOC - Economics

**Core Purpose**: Domain MOC utama untuk navigasi makroekonomi, mencakup dinamika inflasi, kebijakan bank sentral, struktur suku bunga, indikator pertumbuhan agregat, serta analisis ekonomi negara global dan domestik.

---

## 🗺️ Knowledge Structure

### 1. 📈 Dinamika Inflasi & Daya Beli
* **Pengukuran & Indeks Inflation**
  * [[Inflation Measurement Indices (CPI, PPI, PCE)]] — Indeks harga konsumen inti dan umum.
  * [[Inflation Measurement Indices (CPI, PPI, PCE)]] — Indeks harga produsen tingkat grosir.
  * [[Inflation Measurement Indices (CPI, PPI, PCE)]] — Pengukur inflasi acuan The Fed.
* **Mekanisme & Skenario Inflasi**
  * [[Inflation Dynamics & Scenarios]] — Pemicu inflasi permintaan vs dorongan biaya.
  * [[Inflation Dynamics & Scenarios]] — Spiral umpan balik kenaikan upah dan harga barang.
  * [[Inflation Dynamics & Scenarios]] — Skenario krisis inflasi ekstrem dan stagnasi pertumbuhan.
* **Dampak & Perlindungan Modal**
  * [[Purchasing Power Erosion]] — Penurunan daya beli riil mata uang.
  * [[Inflation-Hedged Assets]] — Komoditas dan aset riil pelindung inflasi.

### 2. 🏦 Kebijakan Moneter, Suku Bunga & Yield Curve
* **Kebijakan Bank Sentral**
  * [[Federal Funds Rate & BI Rate]] — Suku bunga acuan penetap biaya modal.
  * [[Central Bank Liquidity Operations (OMO, QE, QT)]] — Operasi pasar terbuka instrumen likuiditas.
  * [[Central Bank Liquidity Operations (OMO, QE, QT)]] — Ekspansi vs kontraksi neraca bank sentral.
* **Struktur Yield Curve & Resesi**
  * [[Yield Curve Dynamics & Recession Indicators]] — Term structure suku bunga obligasi pemerintah.
  * [[Yield Curve Dynamics & Recession Indicators]] — Kurva imbal hasil terbalik sebagai indikator sinyal resesi.
* **Transmisi ke Valuasi**
  * [[Impact of Rate Hikes on Equity Valuations]] — Dampak pengetatan moneter pada penyesuaian diskon ekuitas.

### 3. 📊 Indikator Kesehatan Makroekonomi
* **Pertumbuhan & Produksi Agregat**
  * [[Economic Growth Indicators (GDP & PMI)]] — Ukuran agregat nilai pasar barang dan jasa akhir.
  * [[Economic Growth Indicators (GDP & PMI)]] — Leading indicator aktivitas bisnis manufaktur dan jasa.
* **Pasar Tenaga Kerja (Labor Market)**
  * [[Labor Market Indicators (NFP & Claims)]] — Data penyerapan tenaga kerja dan pengangguran AS.
  * [[Labor Market Indicators (NFP & Claims)]] — Klaim pengangguran mingguan frekuensi tinggi.
* **Konsumsi & Properti**
  * [[Retail Sales Data]] — Ukuran langsung pengeluaran sektor ritel dan rumah tangga.
  * [[Consumer Sentiment Index]] — Indikator psikologis kepercayaan konsumen.
  * [[Housing Starts & Building Permits]] — Sektor konstruksi sensitif suku bunga.

### 4. 🌍 Ekonomi Negara & Makro Regional
* **🇺🇸 Ekonomi Amerika Serikat (US Economics)**
  * [[US Debt Ceiling & Treasury Issuance]] — Plafon utang AS dan penerbitan obligasi Treasury.
  * [[USD Index (DXY) & Global Liquidity]] — Indeks kekuatan Dolar AS dan arus likuiditas global.
* **🇨🇳 Ekonomi Tiongkok (China Economics)**
  * [[PBOC Monetary Policy]] — Instrumen kebijakan moneter PBOC (LPR, RRR cut).
  * [[China Property Sector & Industrial Output]] — Sektor properti dan output industri manufaktur Tiongkok.
* **🇮🇩 Ekonomi Indonesia (Domestic Economics)**
  * [[Cadangan Devisa & Stabilitas Rupiah]] — Intervensi BI dan ketahanan eksternal rupiah.
  * [[APBN, Subsidi, & Defisit Fiskal]] — Postur anggaran belanja negara & peredam kejut fiskal.
  * [[Neraca Perdagangan Komoditas]] — Ekspor-impor komoditas penopang neraca berjalan.
* **🌏 Emerging vs Developed Markets**
  * [[Capital Flows & Foreign Direct Investment (FDI)]] — Arus modal jangka pendek vs investasi riil.
  * [[Current Account Deficit (CAD)]] — Indikator kerentanan defisit transaksi berjalan.

---

## 📌 Dynamic Indexing (Dataview)

```dataview
TABLE type AS Type, status AS Status, file.mtime AS "Last Modified"
FROM #economics OR #macroeconomics OR #indicator
WHERE file.name != this.file.name
SORT file.name ASC
```