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
FirstSeenDate:: 
FirstSeenLocation:: 
Gender:: Male
Home:: [[Iglberg]]
Icon:: 
Job:: 
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
Parent:: 
Race:: [[Human]]
Romance:: [[Helmine]]
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

`=this.Gender` `=this.Race` from `=this.Home`.
Friends with the three men from [[Iglberg]] that died from attack by a [[Peryton]]

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
and [[Volker]]
sort file.name asc
```