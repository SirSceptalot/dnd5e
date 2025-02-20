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
FirstSeenDate:: [[0835-08-26]]
FirstSeenLocation:: [[Alfarin]]
Gender:: female
Home:: [[Alfarin]]
Icon:: 
Job:: Matriarch
LastLocation:: [[Alfarin]]
Leader:: 
Leads:: [[Yushrish]]
MemberOf:: [[Yushrish]]
Offspring:: 
Owns:: 
Parent:: 
Race:: [[Drow]]
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

A `=this.Gender` `=this.Race` from `=this.Home`, matriarch of the [[Yushrish]] family.

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
and [[Rahode Yushrish]]
sort file.name asc
```