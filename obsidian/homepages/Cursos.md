<br/>

```button
name Adicionar curso
type command
action QuickAdd: Adicionar curso
```

<br/>


```dataview 
table without id file.link as Curso, Status, Tópico, Url
from "obsidian/cursos" 
sort file.name asc
```
