---
hide-trail: true
---
# `= this.file.name`
%%
Possible entries: Associate; Birthday; DestroyDate; Destroyed; Enemy; FirstSeenDate; FirstSeenLocation; Gender; Home; Icon; Job; LastLocation; Leads; MemberOf; Offspring; Owns; Parent; Race; Romance; Servant; Serves; Workplace; Worshiper
%%
[FirstSeenDate:: [[0835-10-07]]]
[FirstSeenLocation:: [[Topaz Wand]]]
[Gender:: female]
[Home:: [[Topaz Wand]]]
[Job:: Innkeeper]
[LastLocation:: [[Topaz Wand]]]
[Owns:: [[Topaz Wand]]]
[Race:: [[Human]]]
[Workplace:: [[Topaz Wand]]]


Friendly human magic user, former adventurer.
Now runs the Topaz Wand inn.

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
and [[Elyn]]
sort file.name asc
```