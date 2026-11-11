<%*
let dateTitle = tp.date.now("YYYY-MM-DD");
if (tp.file.title.startsWith("Untitled") || tp.file.title === "") {
  await tp.file.rename(dateTitle);
}
await tp.file.move("10 Inbox/" + tp.file.title);
-%>
---
title: "<% tp.file.title %>"
id: <% tp.date.now("YYYYMMDDHHmmss") %>
aliases: []
type: daily
status: processed
tags:
  - journal/daily
created: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
updated: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
source: internal
related: []
---

# 📅 Daily Log - <% tp.file.title %>

## 💡 Quick Captures & Ide Mental
> [!tip] Petunjuk
> Ide mentah di sini dapat diekstrak menjadi *Atomic Note* menggunakan perintah `/process-inbox`.
* <% tp.file.cursor(1) %>

---

## 🎯 Fokus Aktivitas & Pengembangan Pengetahuan
* [ ] 

---

## 🔗 Catatan & Konsep Yang Dipelajari Hari Ini
* [[

---

## 📊 Summary Catatan Dibuat/Diperbarui (Dataview)
```dataview
LIST FROM !"00 Meta"
WHERE file.cday = date("<% tp.date.now("YYYY-MM-DD") %>") OR file.mday = date("<% tp.date.now("YYYY-MM-DD") %>")
SORT file.mtime DESC