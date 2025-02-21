---
hide-trail: true
---
# `= this.file.name`
[Birthday::]
[DestroyDate::]
[Destroyed:: Yes]
[Enemy::]
[FirstSeenLocation:: [[Horace Ringmann's mansion]]]
[Gender:: male]
[Home:: [[Heidelburg]]]
[Icon::]
[Job::]
[LastLocation::]
[Leader::]
[Leads::]
[MemberOf::]
[Offspring::]
[Owns::]
[Parent::]
[Race:: [[Dwarf]]]
[Romance::]
[Servant::]
[Serves::]
[Workplace::]

---

[[0835-08-07]]: We found a crypt under the house of [[† Horace Ringmann]].
The following comes from the plaque attached to the grave.

*Here lies Ogrim Stormbrow, blessed by Lolth and slain by the servants of the Raven Queen.
Though he lies dead, he may never rest and one day he will find his way back to Aurocondor to re-join the war eternal.*

His ghost or some such nonsense attacked us there.
In his grave we found his remains. His skull was heavily mutated, with 8 eye sockets and elongated canines. This concurs with the plaque's mention of being "blessed by Lolth".

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
and [[† Ogrim Stormbrow]]
sort file.name asc
```