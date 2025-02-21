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
FirstSeenDate:: [[0835-09-21 (alternate timeline)]]
FirstSeenLocation:: 
Gender:: 
Home:: 
Icon:: 
Job:: 
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
Parent:: 
Race:: 
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

Extremely odd creature we encountered and fought while trying to [[Recover Camedyr Baughan]].
No idea what race it was, only that it had some effect that made you forget about it even during combat.

[[0836-04-07]]: we come to the realisation that this creature might be the offspring of a Great Old One. Whoops.

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
and [[The Child]]
sort file.name asc
```