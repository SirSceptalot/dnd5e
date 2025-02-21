---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: [[Exaltators]]]
[FirstSeenLocation:: [[Avelund]]]
[Gender:: female]
[Home:: [[Avelund]]]
[Icon:: ]
[Job:: ]
[LastLocation:: [[Avelund]]]
[Leads:: [[Avelund Resistance]]]
[MemberOf:: [[Avelund Resistance]]]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: [[Human]]]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]

---

A `=this.Gender` `=this.Race` from `=this.Home`.

Allies:
```dataview
list WHERE any(contains(MemberOf, this.MemberOf))
AND MemberOf != NULL
AND file.name != this.file.name
sort file.name asc
```

```dataview
table without id file.link as "Sighting/Interaction", Location
from "10 Journal"
and [[Almira Maiden]]
sort file.name asc
```