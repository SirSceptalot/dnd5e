---
hide-trail: true
---
# `= this.file.name`
[Birthday::]
[DestroyDate::]
[Destroyed:: No]
[Enemy::]
[FirstSeenLocation:: [[Amaroth]]]
[Gender:: male]
[Home:: [[Amaroth]]]
[Icon::]
[Job:: Doctor]
[LastLocation::]
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
[Worshiper::]

---

A `=this.Gender` `=this.Race` from `=this.Home`, mentor of [[Arinya]].

Allies:
```dataview
list FROM "30 Characters"
WHERE any(contains(MemberOf, this.MemberOf))
AND MemberOf != ""
AND file.name != this.file.name
sort file.name asc
```

```dataview
table without id file.link as "Sighting/Interaction", Location
from "10 Journal"
and [[Dr. Kasimir]]
sort file.name asc
```