---
hide-trail: true
---
# `= this.file.name`
%%
Possible entries: Associate; Birthday; DestroyDate; Destroyed; Enemy; FirstSeenDate; FirstSeenLocation; Gender; Home; Icon; Job; LastLocation; Leads; MemberOf; Offspring; Owns; Parent; Race; Romance; Servant; Serves; Workplace; Worshiper
These values are added below. Fill in known info and delete the rest.
Keep the above list intact so you can insert things in the correct alphabetical order when adding back a field if you obtain new information.
%%
[Enemy:: [[Exaltators]]]
[FirstSeenDate:: [[0835-10-13]]]
[FirstSeenLocation:: [[Avelund]]]
[Gender:: male]
[Home:: [[Avelund]]]
[Job:: Smuggler]
[LastLocation:: [[Avelund]]]
[MemberOf:: [[Avelund Resistance]]]
[Race:: [[Human]]]

---

Used to smuggle contraband into Avelund.
During the occupation of the city, he now smuggles people and goods out.

[[0835-10-13]]: We go to his place to introduce ourselves and to indicate that we might be able to use him later.

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
and [[Eugene Grey]]
sort file.name asc
```