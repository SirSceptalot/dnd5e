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
FirstSeenDate:: 
FirstSeenLocation:: 
Gender:: female
Home:: 
Icon:: 
Job:: Deity
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
Parent:: 
Race:: creature
Romance:: 
Servant:: [[† Ogrim Stormbrow]]
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

A `=this.Gender` `=this.Race` from `=this.Home`.

Goddess of spiders, murderers and poison.
Mainly worshiped by dark elves.
Possesses her own domain in the Abyss

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
and [[Lolth]]
sort file.name asc
```