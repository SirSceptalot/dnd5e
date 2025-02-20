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
FirstSeenDate:: [[0835-08-03]]
FirstSeenLocation:: [[Sunshine Sanctuary for Wayward Dragons]]
Gender:: female
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
Serves:: [[Arinya]]
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

A `=this.Gender` `=this.Race` from the `=this.FirstSeenLocation`, adopted by [[Arinya]] on [[0835-08-03]].

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
and [[Fiona]]
sort file.name asc
```