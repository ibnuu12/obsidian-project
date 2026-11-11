<%*
let title = tp.file.title;
if (title.startsWith("Untitled") || title === "" || title.startsWith("Untitled ")) {
  let promptTitle = await tp.system.prompt("Judul Permanent Note (Title Case):", "", false);
  title = promptTitle && promptTitle.trim() !== "" ? promptTitle.trim() : "Konsep Baru";
  await tp.file.rename(title);
}

await tp.file.move("30 Notes/" + tp.file.title);
-%>
---
title: "<% tp.file.title %>"
id: <% tp.date.now("YYYYMMDDHHmmss") %>
aliases: []
type: permanent
status: evergreen
tags:
  - zettel/permanent
  - permanent
created: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
updated: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
source: 
related: []
---

# 🧠 <% tp.file.title %>

> [!abstract] Inti Konsep ($1 \text{ Catatan} = 1 \text{ Ide}$)
> <% tp.file.cursor(1) %>

---

## 📌 Penjelasan & Sintesis Detail


---

## 🔗 Related Notes (Outgoing Links: 2-10)
* [[
* [[

---

## 📚 Referensi & Literature Source
* [[