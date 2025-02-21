---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
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
[Race:: [[Warforged]]]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]

---

A `=this.Gender` `=this.Race` from `=this.Home`.

[[0836-02-08]]: Dominated by [[Hadak]]
[[0836-03-23]]: Has been freed from Hadak, but has become hostile towards [[Skogsland]] and [[Paragon]] because of information he was given by Hadak.
In the process of freeing him, he was also killed but revived at once.

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
and [[Render]]
sort file.name asc
```