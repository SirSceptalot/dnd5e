---
hide-trail: true
---
[Ally:: ]
[Associate:: ]
[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: ]
[FirstSeenDate:: [[0835-09-02]]]
[FirstSeenLocation:: [[Mercenary Ring]]]
[Gender:: male]
[Home:: ]
[Icon:: ]
[Job:: Mercenary]
[LastLocation:: ]
[Leader:: ]
[Leads:: [[Band of the Hawk]]]
[MemberOf:: [[Band of the Hawk]]]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: [[Human]]]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]
# `= this.file.name`
---

Known as "The Hawk", this man leads the [[Band of the Hawk]].

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
and [[Griffith]]
sort file.name asc
```