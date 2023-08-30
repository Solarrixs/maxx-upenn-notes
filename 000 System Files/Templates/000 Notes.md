---
date: <% tp.file.creation_date("YYYY-MM-DD") %>
type: <% tp.system.suggester(["note ", "MOC"], ["note", "MOC"]) %>
<% tp.system.suggester(["tags: ", "tags: ankify"], ["tags: ", "tags: ankify"]) %>
---

<% tp.file.cursor(1) %>