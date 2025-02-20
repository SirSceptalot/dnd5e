---
hide-trail: true
---
%%
Birthday:: 
DestroyDate:: 
Destroyed:: No
Enemy:: 
FirstSeenLocation:: [[The Singed Hare]]
Gender:: male
Home:: [[Heidelburg]]
Icon:: 
Job:: Innkeeper
LastLocation:: [[The Singed Hare]]
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: [[The Singed Hare]]
Parent:: 
Race:: [[Elf]]
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

A `=this.Gender` `=this.Race` from `=this.Home`, owns [[The Singed Hare]]

Allies:
```dataview
list WHERE any(contains(MemberOf, this.MemberOf))
AND MemberOf != NULL
AND file.name != this.file.name
sort file.name asc
```

```dataview
table without id file.link as "Sighting/Interaction", Location
from "10 Journal"
and [[Eliorod]]
sort file.name asc
```