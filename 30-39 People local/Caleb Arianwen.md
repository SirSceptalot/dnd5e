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
FirstSeenDate:: [[0835-09-06]]
FirstSeenLocation:: 
Gender:: male
Home:: [[Collegento]]
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
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

[[0835-09-06]]: A `=this.Race` from `=this.Home`, he wishes to hire us to accompany him to the [[StormMaw Tribe]] to initiate a trade deal.

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
and [[Caleb Arianwen]]
sort file.name asc
```