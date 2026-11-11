<%*
let title = tp.file.title;
if (title.startsWith("Untitled") || title === "" || title.startsWith("Untitled ")) {
  let promptTitle = await tp.system.prompt("Topik / Domain MOC (contoh: Distributed Systems):", "", false);
  title = promptTitle && promptTitle.trim() !== "" ? promptTitle.trim() : "New Topic MOC";
  await tp.file.rename("MOC - " + title);
}

await tp.file.move("20 MOCs/" + tp.file.title);
-%>
---
title: "<% tp.file.title %>"
id: <% tp.date.now("YYYYMMDDHHmmss") %>
aliases: []
type: moc
status: active
tags:
  - zettel/moc
created: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
updated: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
source: internal
related: []
---

# 🗺️ <% tp.file.title %>

> [!abstract] Overview
> Peta navigasi terstruktur untuk domain pengetahuan ini. *(MOC ini tidak menyimpan konten ide, hanya indeks navigasi).*

---

## 🎯 Core Concepts
* [[

---

## 🔗 Related Concepts & Sub-MOCs
* [[

---

## 🛣️ Learning Order & Roadmap
1. [[

---

## 📚 Reference Notes & Projects
* [[

---

## ❓ Suggested Questions & Knowledge Gaps
* ---

## 🔍 Automated Topic Index (Dataview)
```dataview
TABLE file.mtime AS "Last Modified", tags AS "Tags"
FROM #zettel AND !"00 Meta" AND !"20 MOCs"
WHERE contains(file.outlinks, this.file.link) OR contains(this.file.outlinks, file.link)
SORT file.name ASC