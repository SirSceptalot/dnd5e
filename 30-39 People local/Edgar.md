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
[Job:: Familiar]
[LastLocation:: ]
[Leads:: ]
[MemberOf:: ""]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: [[Raven]]]
[Romance:: ]
[Servant:: ]
[Serves:: [[Arinya]]]
[Workplace:: ]

---

A `=this.Gender` `=this.Race`.
Was bonded to [[Arinya]] by a card from a [[Deck of Many Things]].
His origin is unknown besides that.

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
and [[Edgar]]
sort file.name asc
```