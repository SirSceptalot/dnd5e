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
Icon:: [[Bahamut]]
Job:: Cleric
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
Parent:: 
Race:: [[Dragonborn]]
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
and [[Naarhunthes]]
sort file.name asc
```