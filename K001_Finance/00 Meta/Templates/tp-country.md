---
id: "<% tp.date.now("YYYYMMDDHHmm") %>"
title: "<% tp.file.title %>"
aliases: []
tags:
  - country
type: reference
status: active
created: "<% tp.file.creation_date("YYYY-MM-DD HH:mm") %>"
updated: "<% tp.file.last_modified_date("YYYY-MM-DD HH:mm") %>"
currency: ""
source: ""
related: []
---
<%*
let title = tp.file.title;
if (title.startsWith("Untitled") || title === "") {
    title = await tp.system.prompt("Country Name:");
    await tp.file.rename("Country - " + title);
}
await tp.file.move("30 Notes/" + tp.file.title);
-%>
# <% title %>

## 🌐 Macro Highlights
- **GDP Growth:** [[GDP]]
- **Policy Rate:** [[Interest Rate]]
- **Inflation Rate:** [[Inflation]]
- **Currency:** [[FX]]
- **Trade Balance:** [[Trade Balance]]

## 📊 Core Risk & Structure
- **Debt-to-GDP:** [[Debt to GDP]]
- **Political Risk:** - **Major Industries:** - **Exports:** [[Exports]]
- **Imports:** [[Imports]]

## 🏢 Key Companies
```dataview
TABLE sector AS Sector, status AS Status
FROM #company
WHERE contains(file.outlinks, this.file.link)