---
hide-trail: true
---
%%
Ally:: 
Associate:: 
Birthday:: 
DestroyDate:: 
Destroyed:: No
Enemy:: 
FirstSeenDate:: [[0835-08-19]]
FirstSeenLocation:: the material plane
Gender:: male
Home:: [[Avandar]]
Icon:: 
Job:: 
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
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

A `=this.Gender` `=this.Race` from `=this.Home`.

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
and [[Feyris]]
sort file.name asc
```