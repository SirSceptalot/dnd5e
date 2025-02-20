---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: [[0836-04-11]]]
[Destroyed:: No]
[Enemy:: ]
[Gender:: male]
[Home:: ]
[Icon:: ]
[Job:: ]
[LastLocation:: ]
[Leads:: ]
[MemberOf:: ""]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: Human]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]

---

![[0836-04-11#Encounter with Vestalius]]

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
and [[Vestalius]]
sort file.name asc
```