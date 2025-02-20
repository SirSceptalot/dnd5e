---
hide-trail: true
---
# `= this.file.name`
%%
Ally:: 
Associate:: 
Birthday:: 
DestroyDate:: 
Destroyed:: No
Enemy:: 
%%
[FirstSeenDate:: [[0835-09-20 (continued)]]]
[FirstSeenLocation:: [[Temple of Asmodeus in Collegento]]]
%%
%%
[Gender:: female]
[Home:: [[Collegento]]]
[Icon:: [[Asmodeus]]]
[Job:: Cleric]
%%
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
Parent:: 
%%
[Race:: [[Human]]]
%%
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%

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
and [[Runa]]
sort file.name asc
```