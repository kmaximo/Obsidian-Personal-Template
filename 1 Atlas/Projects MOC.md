up:: [[HOME]]
tags:: #map #project   

# Projetos 

>[!abstract]+ Lista com todos os projetos 
```dataview 
table without id file.link as Project,
Subtitle as Description, Version, Status, Completed_on
from #project  and !"1 Atlas" and !"9 Setup"

sort Project desc
```
