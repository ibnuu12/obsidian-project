---
id: 20260728140002
title: Master Map of Content
aliases:
  - Master MOC K003
  - Home Personal
tags:
  - zettel/moc
  - zettel/master
type: moc
status: active
created: 2026-07-28 14:00
updated: 2026-07-28 14:00
source: ""
related: []
---

# Master Map of Content (Vault K003)

**Core Purpose**: Dashboard pusat navigasi utama untuk Manajemen Kehidupan Pribadi, Habit Tracking, Jurnal Harian, & Manajemen Proyek.

---

## Core Domain Navigation

| Domain Utama              | Deskripsi & Cakupan Pengetahuan                           | MOC Target                                               |
| :------------------------ | :-------------------------------------------------------- | :------------------------------------------------------- |
| **Daily Notes & Journal** | Catatan harian, refleksi, log aktivitas, & habit tracking | [[40 Daily/Daily Log\|Daily Log]]                        |
| **Goals & OKRs**          | Penetapan target jangka pendek/panjang dan kerangka OKR   | [[20 MOCs/MOC - Goals & Vision\|MOC - Goals & Vision]]   |
| **Project Management**    | Status proyek berjalan, Kanban, & Resource allocation     | [[20 MOCs/MOC - Projects\|MOC - Projects]]               |
| **Ideas & Incubator**     | Kumpulan ide acak, aspirasi, & hal-hal untuk dieksplorasi | [[20 MOCs/MOC - Ideas Incubator\|MOC - Ideas Incubator]] |

---

## Cross-Vault Navigator

| Destination    | Keterangan                             | Shortcut                                                                                                   |
| :------------- | :------------------------------------- | :--------------------------------------------------------------------------------------------------------- |
| **Vault K001** | Finance, Macroeconomics, & Investing   | [Buka Vault K001_Finance](obsidian://open?vault=K001_Finance&file=20%20MOCs%2FMaster%20Map%20of%20Content) |
| **Vault K002** | Technology, Architecture & Engineering | [Buka Vault K002_Tech](obsidian://open?vault=K002_Tech&file=20%20MOCs%2FMaster%20Map%20of%20Content)       |

---

## Active Indexing (Dataview)

```dataview
TABLE type AS Type, file.mtime AS "Last Modified"
FROM #zettel/moc AND !"00 Meta"
WHERE file.name != this.file.name
SORT file.name ASC
```

