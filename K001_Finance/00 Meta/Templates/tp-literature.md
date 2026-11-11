<%*
let title = tp.file.title;
if (title.startsWith("Untitled") || title === "" || title.startsWith("Untitled ")) {
  let promptTitle = await tp.system.prompt("Judul Buku / Artikel / Sumber:");
  title = promptTitle && promptTitle.trim() !== "" ? promptTitle.trim() : "Literature Source";
  await tp.file.rename("Lit - " + title);
}

let author = await tp.system.prompt("Penulis / Pembuat (Opsional):", "", false);
let cleanAuthor = author && author.trim() !== "" ? author.trim() : "Unknown";

await tp.file.move("30 Notes/" + tp.file.title);
-%>
---
title: "Lit - <% title %>"
id: <% tp.date.now("YYYYMMDDHHmmss") %>
aliases: []
type: literature
status: reading
tags:
  - zettel/literature
  - literature
author: "<% cleanAuthor %>"
source: 
created: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
updated: <% tp.file.creation_date("YYYY-MM-DD HH:mm") %>
related: []
---

# 📚 Lit - <% title %>

> [!info] Metadata Referensi
> **Penulis/Kreator:** <% cleanAuthor %>  
> **Sumber URL/Ref:** > **Status:** #reading

---

## 📑 Ringkasan Eksekutif
* ## 🔑 Poin-Poin Kunci & Kutipan Mentah (Level 2-3)
<% tp.file.cursor(1) %>

---

## 💡 Ide & Sintesis Permanent Note (Level 4-5)
> [!tip] Petunjuk Ekstraksi
> Jalankan perintah `/atomic` atau `/permanent` untuk mengekstrak poin di bawah menjadi *Atomic Notes* di **30 Notes/**.

* ---

## 🔗 Related Notes
* [[