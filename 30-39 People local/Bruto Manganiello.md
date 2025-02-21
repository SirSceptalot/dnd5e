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
FirstSeenLocation:: [[Mineral Minded]]
Gender:: male
Home:: [[Mineral Minded]]
Icon:: 
Job:: Blacksmith
LastLocation:: 
Leader:: 
Leads:: [[Blacksmith guild of Ermedes]]
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

A `=this.Gender` `=this.Race` from [[Ermedes]]
His business is located in the [[Goosed]] district.

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
and [[Bruto Manganiello]]
sort file.name asc
```