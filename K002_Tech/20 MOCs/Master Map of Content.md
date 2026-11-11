---
id: 20260728140001
title: Master Map of Content
aliases:
  - Master MOC K002
  - Home Tech
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

# Master Map of Content (Vault K002)

**Core Purpose**: Dashboard pusat navigasi utama untuk menghubungkan domain konten Keahlian Teknis: Software Engineering, System Architecture, AI Development, & DevOps.

---

## Core Domain Navigation

| Domain Utama             | Deskripsi & Cakupan Pengetahuan                                 | MOC Target                                                         |
| :----------------------- | :-------------------------------------------------------------- | :----------------------------------------------------------------- |
| **Software Engineering** | Algoritma, Struktur Data, Design Patterns, dan Clean Code       | [[20 MOCs/MOC - Software Engineering\|MOC - Software Engineering]] |
| **System Architecture**  | Microservices, Scalability, System Design, & Database Internals | [[20 MOCs/MOC - System Architecture\|MOC - System Architecture]]   |
| **AI Development**       | Machine Learning, LLMs, Prompt Engineering, & AI Agents         | [[20 MOCs/MOC - AI Development\|MOC - AI Development]]             |
| **DevOps & Infra**       | CI/CD, Cloud Infrastructure, Docker, & Kubernetes               | [[20 MOCs/MOC - DevOps\|MOC - DevOps]]                             |

---

## Cross-Vault Navigator

| Destination    | Keterangan                           | Shortcut                                                                                                     |
| :------------- | :----------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| **Vault K001** | Finance, Macroeconomics, & Investing | [Buka Vault K001_Finance](obsidian://open?vault=K001_Finance&file=20%20MOCs%2FMaster%20Map%20of%20Content)   |
| **Vault K003** | Personal Life & Projects             | [Buka Vault K003_Personal](obsidian://open?vault=K003_Personal&file=20%20MOCs%2FMaster%20Map%20of%20Content) |

---

## Active Indexing (Dataview)

```dataview
TABLE type AS Type, file.mtime AS "Last Modified"
FROM #zettel/moc AND !"00 Meta"
WHERE file.name != this.file.name
SORT file.name ASC
```

