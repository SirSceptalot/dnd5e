---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: ]
[Gender:: female]
[Home:: [[Avandar]]]
[Icon:: ]
[Job:: Military]
[LastLocation:: ]
[Leads:: ]
[MemberOf::]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: [[Elf]]]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]

---

A `=this.Gender` `=this.Race` from `=this.Home`.
MemberOf: `=this.MemberOf`

Allies:
```dataview
list FROM "30 Characters"
WHERE any(contains(MemberOf, this.MemberOf))
AND MemberOf != ""
AND file.name != this.file.name
sort file.name asc
```

```dataview
table without id file.link as "Sighting/Interaction", Location
from "10 Journal"
and [[Elanil]]
sort file.name asc
```