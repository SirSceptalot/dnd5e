---
hide-trail: true
---
# `= this.file.name`
%%
Possible entries: Birthday; DestroyDate; Destroyed; Enemy; FirstSeenDate; FirstSeenLocation; Gender; Home; Icon; Job; LastLocation; Leads; MemberOf; Offspring; Owns; Parent; Race; Romance; Servant; Serves; Workplace; Worshiper
These values are added below. Fill in known info and delete the rest.
Keep the above list intact so you can insert things in the correct alphabetical order when adding back a field if you obtain new information.
%%
[Destroyed:: No]
[FirstSeenLocation:: [[Avelund mines]]]
[Gender:: male]
[Icon:: [[Erathis]]]
[LastLocation:: [[Avelund]]]
[Race:: [[Deva]]]

---

[[0835-10-14]]: Viantius was held captive by [[Behektur]] in the [[Avelund mines]] as a source of celestial blood, which was used in the production of [[Ambrosia]].

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
and [[Viantius]]
sort file.name asc
```