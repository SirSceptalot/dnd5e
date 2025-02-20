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
FirstSeenDate:: [[0835-08-31]]
FirstSeenLocation:: [[Mineral Minded]]
Gender:: genderless
Home:: 
Icon:: 
Job:: Military
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
Parent:: 
Race:: [[Warforged]]
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

Unknown party in the mission to [[Solve the murder in Ermedes]].
Has at least some magical ability, but does not shy away from close contact either.

[[0835-09-01]]: We manage to apprehend the individual, who turns out to be another [[Warforged]] disguised as a human female.

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
and [[murderer]]
sort file.name asc
```