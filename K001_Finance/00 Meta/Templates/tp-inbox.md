<%*
let title = await tp.system.prompt("Judul Catatan Ringkas (Opsional):", "", false);
let cleanTitle = title && title.trim() !== "" ? title.trim() : "Tangkapan Cepat";

if (!title || title.trim() === "") {
  await tp.file.rename("Inbox " + tp.date.now("YYYYMMDD-HHmmss"));
} else {
  await tp.file.rename("Inbox " + tp.date.now("YYYYMMDD-HHmm") + " - " + cleanTitle);
}

await tp.file.move("10 Inbox/" + tp.file.title);
-%>
---
title: "<% cleanTitle %>"
id: <% tp.date.now("YYYYMMDDHHmmss") %>
aliases: []
type: fleeting
status: unprocessed
tags:
  - zettel/fleeting
  - inbox
created: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
updated: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
source: 
related: []
---

# 💡 <% cleanTitle %>

> [!info] Panduan Pemrosesan
> Catatan ini berada di **10 Inbox/**. Jalankan perintah `/process-inbox` atau `/capture` untuk memecah catatan ini menjadi *Atomic Notes* di **30 Notes/**.

## 📝 Catatan Mentah
<% tp.file.cursor(1) %>

---
## 🔍 Outgoing Link Candidates
* ## 📌 Context / Source Notes
* ```