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
FirstSeenDate:: a certain day
FirstSeenLocation:: [[Gribenwald]]
Gender:: female
Home:: [[Gribenwald]]
Icon:: 
Job:: 
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: 
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

People in [[Little Ivy Wood]] say a ghost haunts the woods.

A number of the lumberjacks tell stories of going into the woods, but facing ever increasing resistance. This seems to be more creepy than harmful though.

*The forest will first start to grow quiet. Those that don't find this eerie enough to return, the shrubs and branches of the forest will try to physically pull you back.
If even that does not deter you, the final warning is the appearance of "the white woman", which has been enough to scare away even the most determined travelers.*

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
and [[White Woman]]
sort file.name asc
```