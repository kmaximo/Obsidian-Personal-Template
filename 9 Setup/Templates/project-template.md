---
Project: {{VALUE:Add Project}}
Subtitle: {{VALUE:Project Subtitle}}
Timespan: {{VALUE:10 Years, 5 Years, 3 Years, 1 Year, 6 Months, 1 Month, 1 Week}}
Completed_on: 
Version: "0.1"
Status: {{VALUE:todo,waiting,in progress,completed,discarded}}
# status: "todo", "waiting", "in progress", "completed", "discarded"
---
up:: [[Projects MOC]]
tags:: #project
___
# {{VALUE:Add Project}}

<!-- Main content of this chapter -->
.


## {{VALUE:Add Project}} - Tasks
<!-- What remains to be done do get the final version? --> 
```dataview
TABLE without id file.link as Task, Bar
from #task and !"Atlas" and !"Setup"
where Project = "{{VALUE:Add Project}}"
and number(Progress) != number(Target)
sort Task desc

```

TOOLS
#conceptsapp #powerbi #procreate
## Feedback
<!-- What remains for you to consider in the draft version? --> 
-**0.14**

## References
<!-- Links to pages not referenced in the content -->
-