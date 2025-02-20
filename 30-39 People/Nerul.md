---
hide-trail: true
aliases: [God of Death]
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

Nerul, God of Death, was a greedy god with a limitless hunger for power.

As his desire to rule the living was constantly prevented by the other gods, he created the undead to rule them instead.

Eventually his insatiable greed was his downfall, and he was defeated by his apprentice, the [[Raven Queen]].

She defeated him and scattered his body to prevent him from reforming.
It's said one or multiple shards of his body are located in the [[Restless Mire]] in [[Ashein]].

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
and [[Nerul]]
sort file.name asc
```