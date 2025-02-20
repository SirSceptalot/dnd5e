---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: [[0835-12-19]]]
[Destroyed:: Yes]
[Gender:: male]
[Home:: [[Amaroth]]]
[Job:: Wizard]
[LastLocation:: at sea, on [[The Earnest]]]
[Race:: [[Human]]]


---

A `=this.Gender` `=this.Race` from `=this.Home`.
Tried to create a permanent circle of teleportation at sea but was killed by his experiments.

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
and [[Jorge]]
sort file.name asc
```