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
FirstSeenDate:: [[0835-07-31]]
FirstSeenLocation:: [[Iglberg]]
Gender:: Female
Home:: [[Iglberg]]
Icon:: 
Job:: Farmer
LastLocation:: [[Iglberg]]
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
Parent:: 
Race:: [[Human]]
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

`=this.Gender` `=this.Race` from `=this.Home`.
Her husband was the first to be killed by the [[Peryton]] that plagued [[Iglberg]].

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
and [[Mina]]
sort file.name asc
```