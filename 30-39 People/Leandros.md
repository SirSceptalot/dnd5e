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
FirstSeenDate:: [[0835-09-19]]
FirstSeenLocation:: [[Temple of Pelor in Collegento]]
Gender:: male
Home:: [[Collegento]]
Icon:: [[Pelor]]
Job:: Cleric
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
Serves:: [[Horacious]]
Workplace:: [[Temple of Pelor in Collegento]]
Worshiper:: 
%%
# `= this.file.name`
---

A `=this.Gender` `=this.Race` from `=this.Home`.
Acolyte in the `=this.Workplace`.

Helped us during the mission to [[Recover Camedyr Baughan]].

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
and [[Leandros]]
sort file.name asc
```