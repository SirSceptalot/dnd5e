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
FirstSeenDate:: [[0835-08-30]]
FirstSeenLocation:: [[Ermedes]]
Gender:: male
Home:: [[Ermedes]]
Icon:: 
Job:: Prince
LastLocation:: 
Leader:: 
Leads:: [[Ermedes]]
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

A `=this.Gender` `=this.Race` from `=this.Home`.
Prince of [[Ermedes]] - although I'm not sure why his title isn't "King", since he's the highest authority there.

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
and [[Prassede Altomari]]
sort file.name asc
```