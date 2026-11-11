---
id: 202607241000
title: Master Map of Content
aliases:
  - Master MOC
  - Home
tags:
  - zettel/moc
  - zettel/master
type: moc
status: active
created: 2026-07-24 10:00
updated: 2026-07-24 15:35
source: ""
related: []
---

# Master Map of Content

**Core Purpose**: Dashboard pusat navigasi utama untuk menghubungkan 4 domain konten pengetahuan: Ekonomi Makro, Investasi & Valuasi, Pasar Keuangan & Emiten, serta Metodologi Riset & Model Mental.

---

## Core Domain Navigation

| Domain Utama              | Deskripsi & Cakupan Pengetahuan                                                                | MOC Target                                                                 |
| :------------------------ | :--------------------------------------------------------------------------------------------- | :------------------------------------------------------------------------- |
| **Macroeconomics**        | Inflasi, Suku Bunga, Kebijakan Moneter, Indikator Ekonomi, & Analisis Negara (US, China, ID)   | [[20 MOCs/MOC - Economics\|MOC - Economics]]                               |
| **Investing & Valuation** | Valuasi Saham (DCF, Multiples), Manajemen Portofolio, Pendapatan Tetap, & Manajemen Risiko     | [[20 MOCs/MOC - Investing\|MOC - Investing]]                               |
| **Financial Markets**     | Taksonomi Sektor (GICS), Rotasi Sektoral, & Analisis Fundamental Emiten/Perusahaan             | [[20 MOCs/MOC - Financial Markets\|MOC - Financial Markets]]               |
| **Research & Frameworks** | Kerangka Berpikir (Mental Models), Formulasi Tesis Investasi, & Knowledge Management Lifecycle | [[20 MOCs/MOC - Research & Mental Models\|MOC - Research & Mental Models]] |

---

## Core Domain Overview

* [[20 MOCs/MOC - Economics|MOC - Economics]] Pusat navigasi makroekonomi, kebijakan sentral, indikator agregat, dan ekonomi global.
* [[20 MOCs/MOC - Investing|MOC - Investing]] Pusat kalkulasi nilai intrinsik, konstruksi portofolio, dan pengukuran risiko modal.
* [[20 MOCs/MOC - Financial Markets|MOC - Financial Markets]] Pusat pengelompokan sektor bisnis dan analisis kinerja fundamental perusahaan.
* [[20 MOCs/MOC - Research & Mental Models|MOC - Research & Mental Models]] Pusat kerangka keputusan rasional, pengujian tesis, dan siklus pengetahuan.

---

## Cross-Vault Navigator

| Destination    | Keterangan                             | Shortcut                                                                                                     |
| :------------- | :------------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| **Vault K002** | Technology, Architecture & Engineering | [Buka Vault K002_Tech](obsidian://open?vault=K002_Tech&file=20%20MOCs%2FMaster%20Map%20of%20Content)         |
| **Vault K003** | Personal Life & Projects               | [Buka Vault K003_Personal](obsidian://open?vault=K003_Personal&file=20%20MOCs%2FMaster%20Map%20of%20Content) |

---

## Active Indexing (Dataview)

```dataview
TABLE type AS Type, file.mtime AS "Last Modified"
FROM #zettel/moc AND !"00 Meta"
WHERE file.name != this.file.name
SORT file.name ASC
```
