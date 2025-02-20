---
hide-trail: true
---
[Birthday::]
[DestroyDate::]
[Destroyed:: No]
[Enemy::]
[FirstSeenLocation:: [[Ermedes]]]
[Gender:: male]
[Home:: [[Ermedes]]]
[Icon::]
[Job:: Military]
[LastLocation::]
[Leader::]
[Leads::]
[MemberOf::]
[Offspring::]
[Owns::]
[Parent::]
[Race:: [[Elf]]]
[Romance::]
Servant:: 
Serves:: [[Prassede Altomari]]
Workplace:: 
# `= this.file.name`
---

A `=this.Gender` `=this.Race` from `=this.Home`.
In charge of the guard/military forces in [[Ermedes]] for the last 100-ish years.
While dealing with him, he strikes me as a morally sound man.

Allies:
```dataview
list FROM "30 Characters"
WHERE any(contains(MemberOf, this.MemberOf))
AND MemberOf != NULL
AND file.name != this.file.name
sort file.name asc
```

```dataview
table without id file.link as "Sighting/Interaction", Location
from "10 Journal"
and [[Abenzio Iacovone]]
sort file.name asc
```