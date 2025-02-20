---
hide-trail: true
---
%%
Ally:: 
Associate:: 
Birthday:: 
DestroyDate:: 
Destroyed:: No
Enemy:: 
FirstSeenDate:: [[0835-08-31]]
FirstSeenLocation:: [[Copperbank]]
Gender:: female
Home:: [[Collegento]]
Icon:: 
Job:: 
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
Parent:: 
Race:: [[Aasimar]]
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

A `=this.Gender` `=this.Race` from `=this.Home` that we rescued from the brothel [[Swift Finish]].

She comes from a tiny settlement a short while from [[Collegento]], another one of the free cities, where she used the limited magic in her [[Aasimar]] blood to study as healer.

The settlement where she lives is outside the city limits, which technically makes it part of [[Ashein]].

She was kidnapped on her way home from school.

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
and [[Ephemera]]
sort file.name asc
```