---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: Early March 836]
[Destroyed:: Yes]
[Enemy:: ]
[Gender:: male]
[Home:: [[Ekholm]]]
[Icon:: ]
[Job:: Innkeeper]
[LastLocation:: [[The Welcoming Gipsy]]]
[Leads:: ]
[MemberOf:: ]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: creature]
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
and [[Zuri]]
sort file.name asc
```