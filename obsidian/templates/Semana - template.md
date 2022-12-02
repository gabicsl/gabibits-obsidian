---
uuid: <% tp.date.now("YYYYMMDDHHmmss") %>
created: <% tp.file.creation_date("YYYY-MM-DDTHH:mm:ss") %>
updated: <% tp.file.last_modified_date("YYYY-MM-DDTHH:mm:ss") %>
alias: 
---


# 📋 Tarefas

```tasks
not done
due before in 1 week
sort by due
```

<br>

---

<br>

# 🗓️ Notas diárias

```dataview
LIST
FROM "obsidian/journal/dailynote"
WHERE file.ctime >= date(today) - dur(7 days)
```


<br>

# 🌻 Reflexão da Semana

## 3 coisas legais nessa semana
- 
- 
- 

## O que fazer diferente na semana que vem?
