---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: ]
[Gender:: male]
[Home:: ]
[Icon:: ]
[Job:: ]
[LastLocation:: ]
[Leads:: ]
[MemberOf:: ]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: [[Eladrin]]]
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
and [[Taliesin]]
sort file.name asc
```