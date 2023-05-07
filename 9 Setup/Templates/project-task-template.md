---
<%* 
const tag = "#project";
const filteredFiles = app.vault.getMarkdownFiles().filter(file => {  
	const tags = tp.obsidian.getAllTags(app.metadataCache.getFileCache(file));  
	return tags.includes(tag);  
});  
const project = (await tp.system.suggester((file) => file.basename, filteredFiles)).basename;
_%>
Project: <% project %>
Task: {{VALUE:Add Task Project}}
Timespan: {{VALUE:10 Years, 5 Years, 3 Years, 1 Year, 6 Months, 1 Month, 1 Week}}
Type:
Progress: 0
Target: {{VALUE:Target (number)}}
---
up:: [[<% project %>]]
tags:: #task
___
%%
Bar:: `$= dv.view('progress-bar', {file: '{{VALUE:Add Task Project}}'})`
%%
# {{VALUE:Add Task Project}}

<!-- What remains to be done do get the final version? --> 

- [ ] Prepare final version 
- [ ] Publish on GitHub
- [ ] Review and revise

## References
<!-- Links to pages not referenced in the content -->
-