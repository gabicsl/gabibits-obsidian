<br/>

```button
name Adicionar projeto
type command
action QuickAdd: Adicionar projeto
```

<br/>


```dataview
TABLE without id file.link as Projeto, length(file.tasks.text) as Total, length(filter(file.tasks.completed, (t) => t = true)) AS Concluído, "<progress value='" + (length(filter(file.tasks.completed, (t) => t = true)) / length(file.tasks.text)) * 100 + "' max='100'></progress>" AS Progresso, status
FROM "obsidian/projetos"
WHERE file.tasks
sort file.name asc
```