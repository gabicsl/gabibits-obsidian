<br>

```button
name Adicionar novo livro
type command
action QuickAdd: Adicionar livro
```

<br>
<br>

```dataview 
table without id ("![coverimg|100](" + Capa + ")") as Capa, file.link as Título, Autor, Status, (Páginas + " p.") as Páginas, Nota, ( "![progresso + " + (round((páginasLidas/Páginas)*100)) + " %](https://progress-bar.dev/" + (round((páginasLidas/Páginas)*100)) + "/)" ) AS Progresso
from "obsidian/livros" 
sort file.name asc
```