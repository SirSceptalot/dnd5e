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
[Race:: [[Warforged]]]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]

---

The first ever Warforged. She's been locked in isolation by her creators in the [[Workshop]] where she was crafted, and has since replaced her lower extremities by some sort of mobility platform consisting of 8 spidery legs.

She did these modifications together with another [[Warforged]] called [[Ronin]] and the [[Omnissiah]], a shard of the machine god.

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
and [[Weiss]]
sort file.name asc
```