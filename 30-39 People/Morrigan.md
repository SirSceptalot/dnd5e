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
[Job:: deity]
[LastLocation:: ]
[Leads:: ]
[MemberOf:: ""]
[Offspring:: ]
[Owns:: ]
[Parent:: [[Raven Queen]]]
[Race:: creature]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]

---

Handmaiden of the [[Raven Queen]].
Shard of Divinity, created from the [[Raven Queen]].

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
and [[Morrigan]]
sort file.name asc
```