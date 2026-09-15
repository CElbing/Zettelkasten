<%* 
	let title = tp.file.title;
	if(title.startsWith("Untitled")){
		title = await tp.system.prompt("Title");
		await tp.file.rename(title);
	}
%>
Date of Origin: <% tp.file.creation_date() %>
Recent Changes: <% tp.file.last_modified_date() %>
Tags:

---

