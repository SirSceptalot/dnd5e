```dataview
table without id Job, rows.Home as Location, rows.file.link as Name
where Job != NULL
sort Job asc, Home asc, file.link asc
group by Job
```
