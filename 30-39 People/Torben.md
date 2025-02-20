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
FirstSeenLocation:: [[Redcap Boots]]
Gender:: male
Home:: [[Iglberg]]
Icon:: 
Job:: Innkeeper
LastLocation:: [[Iglberg]]
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: [[Redcap Boots]]
Parent:: 
Race:: [[Human]]
Romance:: [[Galiéna]]
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

A `=this.Gender` `=this.Race` from `=this.Home`.
Owns [[Redcap Boots]] and is married to [[Galiéna]].

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
and [[Torben]]
sort file.name asc
```