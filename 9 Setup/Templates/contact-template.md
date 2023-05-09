---
<%* 
const hasTitle = !tp.file.title.startsWith("Untitled");
let title;
if (!hasTitle){
	title = await tp.system.prompt("Nome:");
	await tp.file.rename(title);
	await tp.file.move("2 Cards/People/"+title);
} else {
	title = tp.file.title;
}
let email = await tp.system.prompt("E-Mail:")
console.log(email)
email = email.toLowerCase()
let telefone = await tp.system.prompt("Qual telefone:")
console.log(telefone)

_%>
name: <% title %>
email: <% email %>
telefone: <% telefone %>

---
up:: [[Contact MOC]]
tags:: #person/contact  
___
## 🧍 - Informação de contato
- Nome: <% title %>
- Email: <% email %>
- Telefone: <% telefone %>
___
### 📓 - Notas
- <% tp.file.cursor() %>
