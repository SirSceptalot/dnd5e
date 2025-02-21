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
FirstSeenLocation:: the material plane
Gender:: Male
Home:: 
Icon:: 
Job:: Archmage of Culture
LastLocation:: 
Leader:: 
Leads:: 
MemberOf::  [[Council of Archmages]]
Offspring:: 
Owns:: 
Parent:: 
Race:: creature
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
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
and [[Elostrum]]
sort file.name asc
```