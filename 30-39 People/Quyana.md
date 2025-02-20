---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: ]
[Gender:: female]
[Home:: ]
[Icon:: ]
[Job:: First Mate]
[LastLocation:: ]
[Leads:: ]
[MemberOf:: ""]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: [[Half-Elf]]]
[Romance:: ]
[Servant:: ]
[Serves:: [[Filaurel]]]
[Workplace:: [[Dauntless Explorer]]]

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
and [[Quyana]]
sort file.name asc
```