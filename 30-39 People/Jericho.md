---
hide-trail: true
---
# `= this.file.name`
%%
Possible entries: Associate; Birthday; DestroyDate; Destroyed; Enemy; FirstSeenDate; FirstSeenLocation; Gender; Home; Icon; Job; LastLocation; Leads; MemberOf; Offspring; Owns; Parent; Race; Romance; Servant; Serves; Workplace; Worshiper
These values are added below. Fill in known info and delete the rest.
Keep the above list intact so you can insert things in the correct alphabetical order when adding back a field if you obtain new information.
%%
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: [[Avelund Resistance]]]
[FirstSeenDate:: [[0835-10-12]]]
[FirstSeenLocation:: [[Avelund]]]
[Gender:: male]
[Job:: Military]
[LastLocation:: [[Avelund]]]
[MemberOf:: [[Exaltators]]]
[Race:: [[Hill Giant]]]
[Serves:: [[Jericho]]]

---

A `=this.Gender` mutated `=this.Race`.
[[0835-10-12]]: He has some sort of trumpet attached to his face with which he can unleash a sonic attack, which I found out the hard way.

---

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
and [[Jericho]]
sort file.name asc
```