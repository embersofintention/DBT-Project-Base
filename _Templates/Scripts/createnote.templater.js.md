<%* 
// createnote.templater.js file
let newNoteTitle = "New Note " + moment().format("YYYY-MM-DD");
let newNoteContent = "---\ntags: new-note\n---\n\n# " + newNoteTitle;
tp.file.create(newNoteTitle, newNoteContent);
%>
