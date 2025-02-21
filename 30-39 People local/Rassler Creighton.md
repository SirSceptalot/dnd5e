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
FirstSeenDate:: a certain day
FirstSeenLocation:: [[Mercenary Ring]]
Gender:: male
Home:: 
Icon:: 
Job:: Mercenary
LastLocation:: [[Mercenary Ring]]
Leader:: 
Leads:: [[Black Marauders]]
MemberOf:: [[Black Marauders]]
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

A `=this.Gender` `=this.Race`, leader of the [[Black Marauders]]

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
and [[Rassler Creighton]]
sort file.name asc
```