<%*
let title = tp.file.title;
if (title.startsWith("Untitled") || title === "" || title.startsWith("Untitled ")) {
  let promptTitle = await tp.system.prompt("Judul Master MOC (Default: Master MOC):", "", false);
  title = promptTitle && promptTitle.trim() !== "" ? promptTitle.trim() : "Master MOC";
  await tp.file.rename(title);
}

await tp.file.move("20 MOCs/" + tp.file.title);
-%>
---
title: "<% tp.file.title %>"
id: <% tp.date.now("YYYYMMDDHHmmss") %>
aliases:
  - Main Index
  - Knowledge Hub
type: master-moc
status: active
tags:
  - zettel/moc
  - zettel/master
created: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
updated: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
source: internal
related: []
---

# 🧠 <% tp.file.title %>

> [!abstract] Core Purpose
> High-level dashboard for navigating domains, active projects, and core knowledge structures.

---

## 🗺️ Knowledge Domains (Domain MOCs)
* [[MOC - Technology]] — Software, development, tools, and systems.
* [[MOC - Productivity]] — PKM, workflows, systems, and time management.
* [[MOC - Philosophy]] — Models, ethics, decision-making, and mental frameworks.
* [[MOC - Health]] — Fitness, nutrition, mental health, and sleep.

---

## 🚀 Active Projects & Deliverables
* [[Project - Zettelkasten Setup]] — Vault optimization and workflow scripts.
* [[Writing - Essay Draft]] — Current writing pieces in development.

---

## 📊 Automated Vault Index (Dataview)

### 📌 All Sub-MOCs
```dataview
TABLE file.folder AS "Folder", file.mtime AS "Last Modified"
FROM #zettel/moc AND !"00 Meta"
WHERE file.name != this.file.name
SORT file.name ASC