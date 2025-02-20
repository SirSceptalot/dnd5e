---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: ]
[Gender:: male]
[Home:: [[Esterna]]]
[Icon:: ]
[Job:: Barkeep]
[LastLocation:: ]
[Leads:: ]
[MemberOf:: ""]
[Offspring:: ]
[Owns:: [[Emerald Pipe]]]
[Parent:: ]
[Race:: [[Halfling]]]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: [[Emerald Pipe]]]

---

A `=this.Gender` `=this.Race` from `=this.Home`.

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
and [[Edmond]]
sort file.name asc
```