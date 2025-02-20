---
hide-trail: true
---
# `= this.file.name`

[Birthday::]
[DestroyDate::]
[Destroyed:: No]
[Enemy::]
[Gender:: male]
[Home:: [[Lower Amaroth]]]
[Icon::]
[Job:: Trader]
[LastLocation:: [[Lower Amaroth]]]
[Leads::]
[MemberOf::]
[Offspring::]
[Owns::]
[Parent::]
[Race:: [[Human]]]
[Romance::]
[Servant::]
[Serves::]
[Workplace::]

---

Hired us to clear his warehouse of an infestation of [[Giant Rat|giant rats]].

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
and [[Angus Voorhees]]
sort file.name asc
```