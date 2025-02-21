---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: [[0836-01-17]]]
[Destroyed:: Yes]
[Enemy:: ]
[Gender:: female]
[Home:: ]
[Icon:: ]
[Job:: ]
[LastLocation:: ]
[Leads:: ]
[MemberOf:: ]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: [[Drow]]]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]

---

A `=this.Gender` `=this.Race` from `=this.Home`.
See [[Move the bell of Saint Solar Macharius]].

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
and [[Nathyr]]
sort file.name asc
```