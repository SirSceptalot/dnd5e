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
FirstSeenDate:: a certain day
FirstSeenLocation:: the material plane
Gender:: genderless
Home:: 
Icon:: 
Job:: 
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
Parent:: 
Race:: creature
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

Tharizdun, "chained oblivion".
He was once imprisoned by an alliance of other gods. As far as I know, these were [[Pelor]], [[Asmodeus]], [[Ioun]] and [[Sarenrae]].

[[0835-08-23]]: We see a small chapel in an underground dungeon which may actually be the prison of this monstrous god.


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
and [[Tharizdun]]
sort file.name asc
```