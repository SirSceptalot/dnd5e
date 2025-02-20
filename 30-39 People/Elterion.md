---
hide-trail: true
---
# `= this.file.name`

[Birthday::]
[DestroyDate::]
[Destroyed:: No]
[Enemy::]
[FirstSeenLocation:: [[Avelund]]]
[Gender:: male]
[Home::]
[Icon::]
[Job::]
[LastLocation::]
[Leads::]
[MemberOf::]
[Offspring::]
[Owns::]
[Parent::]
[Race:: [[Void Dragon]]]
[Romance::]
[Servant::]
[Serves::]
[Workplace::]

---

He's been seen several times near [[Aurocondor]].
Is not a classic (metallic or chromatic) dragon, but a seperate type.
Might be able to use Dunemancy.

It's unknown what his link is with [[Aurocondor]], but it's likely his lair is somewhere underwater near it, in a cave some 5 miles from the [[Sacrosanct Monastery]].

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
and [[Elterion]]
sort file.name asc
```