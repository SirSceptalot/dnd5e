---
hide-trail: true
---
# `= this.file.name`
%%
Possible entries: Associate; Birthday; DestroyDate; Destroyed; Enemy; FirstSeenDate; FirstSeenLocation; Gender; Home; Icon; Job; LastLocation; Leads; MemberOf; Offspring; Owns; Parent; Race; Romance; Servant; Serves; Workplace; Worshiper
These values are added below. Fill in known info and delete the rest.
Keep the above list intact so you can insert things in the correct alphabetical order when adding back a field if you obtain new information.
%%
[Associate::]
[Birthday::]
[DestroyDate::]
[Destroyed:: No]
[Enemy::]
[FirstSeenDate:: a certain day]
[FirstSeenLocation:: the material plane]
[Gender:: female]
[Home:: [[Avandar]]]
[Icon::]
[Job::]
[LastLocation::]
[Leads::]
[MemberOf::]
[Offspring::]
[Owns::]
[Parent::]
[Race:: [[High Elf]]]
[Romance::]
[Servant::]
[Serves::]
[Workplace::]
[Worshiper::]

---

A `=this.Gender` `=this.Race` from `=this.Home`.

[[0836-01-18]]: Arinya scries on Faynaigen, the person we're supposed to deliver the [[Bell of Saint Solar Macharius]] to in [[Avandar]]. She turns out to be a very graceful female elf, reading in a library in Avandar. She's of the subrace High Elf.

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
and [[Faynaigen]]
sort file.name asc
```