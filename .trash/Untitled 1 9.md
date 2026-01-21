
```dataview
TABLE
    file.link AS "Note",
    TEMPLATER_BUTTON("Create New Note", "CreateNewNote")
WHERE
    file.day = this.file.day
```





```dataview
TABLE
    file.link AS "Note",
    TEMPLATER_BUTTON("Run Script", "your_script_name_here")
WHERE
    file.day = this.file.day
```

