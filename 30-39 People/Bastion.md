---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: [[0836-02-08]]]
[Destroyed:: Yes]
[Enemy:: ]
[Gender:: genderless]
[Home:: [[Amaroth]]]
[Icon:: ]
[Job:: Military]
[LastLocation:: ]
[Leads:: ]
[MemberOf:: [[Paragon]]]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: [[Warforged Titan]]]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]

---

A `=this.Gender` `=this.Race` from `=this.Home`.
Was destroyed when a magic infused ballista bolt changed his body into the body of [[Hadak]]

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
and [[Bastion]]
sort file.name asc
```