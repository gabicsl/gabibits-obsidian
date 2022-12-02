
```dataview
TABLE WITHOUT ID
  file.link as Date,
  choice(Exercicio > 30, "✅", "❌") as Exercicio,
  choice(Sono > 6, "✅", "❌") as Sono,
  choice(Água >= 2, "✅", "❌") as Água,
  Leitura as Leitura
FROM "obsidian/journal/dailynote"
WHERE file.day <= date(now) AND file.day >= date(now) - dur(7days)
SORT file.day ASC
```