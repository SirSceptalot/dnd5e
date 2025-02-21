---
hide-trail: true
---
# `= this.file.name`
%%
Ally:: 
Associate:: 
Birthday:: 
DestroyDate:: 
Destroyed:: No
Enemy:: 
%%
[FirstSeenDate:: [[0835-09-20 (continued)]]]
[FirstSeenLocation:: [[Nivemer's Stand]]]
[Gender:: male]
%%
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
%%
[Race:: [[Illithid]]]
%%
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%

---

Briefly spotted this character in [[Nivemer's Stand]]. He retreated back through the portal into the [[Far Realms]] after a short conversation.

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
and [[Orestes]]
sort file.name asc
```