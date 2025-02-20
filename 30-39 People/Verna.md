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
FirstSeenDate:: [[0835-09-12]]
FirstSeenLocation:: [[Endike]] mountains
Gender:: female
Home:: 
Icon:: 
Job:: Wife of tribe leader
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: [[StormMaw Tribe]]
Offspring:: 
Owns:: 
Parent:: 
Race:: [[Goliath]]
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

Wife of the [[StormMaw Tribe]] chief.
I defeated her in a friendly wrestling match on [[0835-09-12]] in order to help establish trade agreements between the tribe and [[Caleb Arianwen]] (see mission log [[Expedition to StormMaw Tribe]]).

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
and [[Verna]]
sort file.name asc
```