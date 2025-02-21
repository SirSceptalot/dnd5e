---
hide-trail: true
---
# `= this.file.name`
%%
Possible entries: Associate; Birthday; DestroyDate; Destroyed; Enemy; FirstSeenDate; FirstSeenLocation; Gender; Home; Icon; Job; LastLocation; Leads; MemberOf; Offspring; Owns; Parent; Race; Romance; Servant; Serves; Workplace; Worshiper
These values are added below. Fill in known info and delete the rest.
Keep the above list intact so you can insert things in the correct alphabetical order when adding back a field if you obtain new information.
%%
[Enemy:: [[Behektur]]]
[FirstSeenDate:: [[0835-10-12]]]
[FirstSeenLocation:: [[Avelund]]]
[Gender:: female]
[Home:: [[Avelund]]]
[Job:: Wisdom]
[LastLocation:: [[Avelund]]]
[MemberOf:: [[Avelund Resistance]]]
[Race:: [[Human]]]

---

[[0835-10-12]]: She's tending to the massive injuries [[Cleve Pabst]] has sustained from being broken on the wheel.
We help her tend to him.

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
and [[Bertie Bennet]]
sort file.name asc
```