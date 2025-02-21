---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: ]
[Gender:: genderless]
[Home:: [[Amaroth]]]
[Icon:: ]
[Job:: Military]
[LastLocation:: ]
[Leads:: ]
[MemberOf:: [[Vanguard]]]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: Warforged]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]

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
and [[Sentinel]]
sort file.name asc
```