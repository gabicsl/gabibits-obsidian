---
creation date: <% tp.file.creation_date() %>
modification date: <%+ tp.file.last_modified_date("dddd Do MMMM YYYY HH:mm:ss") %>
week: <% tp.date.now("YYYY-WW") %>

---


<< [[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>]] | [[<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "YYYY-MM-DD") %>]]>>

<br>

```dataviewjs
var a = moment().startOf('day');
var b = moment().endOf('day');

var n = moment()
var t = moment().startOf('day');

let q =  b.diff(a, 'days');
let p =  b.diff(t, 'days');
let r =  t.diff(a, 'days');

let h = n.diff(a, 'hours');
let i = b.diff(a, 'hours');
let j =  b.diff(t, 'hours');

let html = `**PROGRESSO DO DIA**   
<progress style="height:10px;width:50%" value="`+h+`" max="`+i+`"></progress>`

if (r>0 && r<q) {
	html +=  `    **` +(h/i*100).toFixed(0)+`%** | `
	html += +p+` days remaining  ` 
} else if (r==0) {
	html += `    **` +(h/i*100).toFixed(0)+`%**`
} else if (r==q) {
	html += `   Ends today `
} else if (r>q) {
	html += `   Ended `+-j+` hours ago`
}else {
	html += `   `+-r+` days remaining`
}

dv.paragraph(html)
```


## Tarefas para hoje
```tasks
due on today
hide backlink
hide due date
hide edit button
not done
```

<br>

## Agenda


<br>

## Hábitos

**Leitura**:: [[]]
**Sono**:: 0
**Exercicio**:: 0
**Água**:: 0