```ad-city
title: <% tp.file.title %>

!<% tp.frontmatter.image %>

| **Guild** | <% tp.frontmatter.guild %> |
| ---------- | ---------------------------------------- | ----------- | ---------------------------- |
| **Fame**   | <% "⭐".repeat(tp.frontmatter.fame) %>   | **Reach**   | <% tp.frontmatter.reach || "" %>   |    
| **Power**  | <% "⚡".repeat(tp.frontmatter.power) %>  | **Scope**   | <% tp.frontmatter.scope || "" %>   |     
| **Market** | <% "🪙".repeat(tp.frontmatter.market) %> | **Rarities** | <% tp.frontmatter.rarities || "" %> |    
| **Knowledge**           | <% "🌙".repeat(tp.frontmatter.knowledge) %> | **Specialty**                                     | <% tp.frontmatter.specialty || "" %>                      |     
<% tp.frontmatter.tags.map(x => `#${x}`).join(" ") %>
**Factions**
 <% tp.frontmatter.factions?.join("\n") || "" %>
```
