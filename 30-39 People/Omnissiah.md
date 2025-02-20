---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: ]
[Gender:: genderless]
[Home:: ]
[Icon:: ]
[Job:: ]
[LastLocation:: ]
[Leads:: ]
[MemberOf:: ""]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: creature]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]

---

omnisiah kn check:
aspect/deel van de god van de machine
godheid die gevochten heeft in the calamity waar heel veel goden gebroken zijn geweest
de machine god broke as well, and the omnisiah is a part of him. It's a shard of a god.

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
and [[Omnisiah]]
sort file.name asc
```