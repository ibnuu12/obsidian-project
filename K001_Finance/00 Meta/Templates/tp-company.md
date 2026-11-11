---
id: "<% tp.date.now("YYYYMMDDHHmm") %>"
title: "<% tp.file.title %>"
aliases: []
tags:
  - company
  - status/watching
type: reference
status: active
created: "<% tp.file.creation_date("YYYY-MM-DD HH:mm") %>"
updated: "<% tp.file.last_modified_date("YYYY-MM-DD HH:mm") %>"
country: ""
sector: ""
source: ""
related: []
---
<%*
let title = tp.file.title;
if (title.startsWith("Untitled") || title === "") {
    title = await tp.system.prompt("Company Name / Ticker:");
    await tp.file.rename("Company - " + title);
}
await tp.file.move("30 Notes/" + tp.file.title);
-%>
# <% title %>

## 🏢 Business Overview
- **Business Model:** - **Competitive Advantage (Moat):** [[Moat]]
- **Industry:** - **Competitors:** ## 📈 Financial Drivers
- **Revenue Drivers:** - **Cost Structure:** - **Management & Capital Allocation:** ## 🎯 Valuation & Risks
- **Valuation:** [[Equity Valuation]]
- **Catalysts:** - **Risks:** ## 🔗 Related Notes
- Parent Concept: [[MOC - Companies]]
- Country Node: 
- Thesis Link: [[Investment Thesis - <% title %>]]

---
## 💡 Graph Connections
- **Parent Concepts:** [[MOC - Companies]], [[MOC - Valuation]]
- **Child Concepts:** - **Sibling Concepts:** - **Prerequisites:** [[Equity Valuation]], [[Financial Markets]]