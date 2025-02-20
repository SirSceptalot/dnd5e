---
hide-trail: true
---
%%
Birthday:: 
DestroyDate:: 
Destroyed:: No
Enemy:: 
FirstSeenLocation:: [[Ermedes]]
Gender:: female
Home:: [[Ermedes]]
Icon:: 
Job:: Pharmacist
LastLocation:: 
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

A `=this.Gender` `=this.Race` from `=this.Home`. Owns an apothecary in [[Ermedes]]

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
and [[Elana Speratza]]
sort file.name asc
```