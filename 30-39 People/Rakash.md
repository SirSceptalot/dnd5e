---
hide-trail: true
---
# `= this.file.name`
%%
Possible entries: Birthday; DestroyDate; Destroyed; Enemy; FirstSeenDate; FirstSeenLocation; Gender; Home; Icon; Job; LastLocation; Leads; MemberOf; Offspring; Owns; Parent; Race; Romance; Servant; Serves; Workplace; Worshiper
These values are added below. Fill in known info and delete the rest.
Keep the above list intact so you can insert things in the correct alphabetical order when adding back a field if you obtain new information.
%%
[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: ]
[FirstSeenLocation:: [[Ermedes]]]
[Gender:: male]
[Home:: ]
[Icon:: ]
[Job:: ]
[LastLocation:: [[Mercenary Ring]]]
[Leads:: ]
[MemberOf:: [[Jarnbrun]]]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: [[Gnome]]]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]
[Worshiper:: ]

---

A `=this.Gender` `=this.Race` from `=this.Home`.

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
and [[Rakash]]
sort file.name asc
```