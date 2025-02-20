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
[Job:: ]
[LastLocation:: ]
[Leads:: ]
[MemberOf:: ""]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: [[Erinyes]]]
[Romance:: ]
[Servant:: ]
[Serves:: [[Hadak]]]
[Workplace:: ]

---

A `=this.Gender` `=this.Race` from `=this.Home`.
Responsible for the death of [[Bastion]], as she ordered the ballista strike that summoned [[Hadak]] into Bastion's body.

Supports and serves [[Hadak]].

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
and [[Tisiphone]]
sort file.name asc
```