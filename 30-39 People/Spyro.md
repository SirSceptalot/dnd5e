---
hide-trail: true
---
%%
Ally:: [[Tiziano]]
Associate:: 
Birthday:: 
DestroyDate:: 
Destroyed:: No
Enemy:: 
FirstSeenDate:: [[0835-08-03]]
FirstSeenLocation:: [[Sunshine Sanctuary for Wayward Dragons]]
Gender:: male
Home:: 
Icon:: 
Job:: 
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: [[The Experts]]
Offspring:: 
Owns:: 
Parent:: 
Race:: [[Pseudodragon]]
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

A `=this.Gender` `=this.Race` from `=this.Home`.

Originally called Sir Walter the Third, but [[Tiziano]] and him agreed to change his name to Spyro.

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
and [[Spyro]]
sort file.name asc
```