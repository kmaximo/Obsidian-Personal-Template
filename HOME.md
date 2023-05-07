---
cssclass:  maxWidth, dashboard
---

````ad-dashb
title: Menu
color: 3, 135, 36
icon: calendar-today
- ## 
	```button
	name New Contact
	type note(Untitled,split) template
	action contact-template
	color green
	```
- ## 
	```button
	name New Project
	type command
	action QuickAdd: Add Project
	color green
	```
	```button
	name New Task
	type command
	action QuickAdd: Add Task Project
	color green
	```

````

````ad-dashb
title: Personal Management
icon: list
color: 3, 135, 36
- ## ℹ️ About Folders
	- [[+ Sobre o Atlas]]
	- [[+ Sobre Cards]]
	- [[+ Sobre Spaces]]
	- [[+ Sobre Sources]]
	- [[+ Sobre o Setup]]

- ## 🗄️ Assuntos
    `$=dv.list(dv.pages('"1 Atlas"').sort(f=>f.file.mtime.ts,"desc").limit(5).file.link)`
- ## 👨‍👩‍👦 Objetivos
	- [[Family Recipes]]
	- [[Family Calendar]]
	- [[Items to buy]]
- ## 🌅 Viagens 
	- [[Vacations MOC]]
	  `$=dv.list(dv.pages('"5 Spaces/Vacation"').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`

````

````ad-dashb
title: Professional Management
color: 0, 169, 206
icon: briefcase
- ## 🧩 Projects
	```dataview
	table without id file.link as Project,
	Subtitle as Description, Status
	from #project  and !"1 Atlas" and !"9 Setup"
	sort file.mtime desc
	limit 5
	```
- ## 📚 Studies
	- [[Education Plan]]
- ## 💪 Tasks
	- EM DEV
````

````ad-dashb
title: Vault Info
color: 200, 50, 0
icon: file-contract
- ## 🗄️ Recent file updates
	`$=dv.list(dv.pages('').sort(f=>f.file.mtime.ts,"desc").limit(4).file.link)`
- ## 🔖 Tagged:  favorite 
	`$=dv.list(dv.pages('#favorite').sort(f=>f.file.name,"desc").limit(4).file.link)`
- ## 〽️ Stats
	- Total de Arquivos: `$=dv.pages().length`
	- Total de Mídias: `$=dv.pages('"2 Cards/Media"').length`
````
