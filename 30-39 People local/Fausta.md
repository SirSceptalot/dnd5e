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
FirstSeenDate:: [[0835-08-08]]
FirstSeenLocation:: [[Heidelburg Conservatory]]
Gender:: female
Home:: [[Heidelburg]]
Icon:: 
Job:: Librarian
LastLocation:: [[Heidelburg Conservatory]] 
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
Parent:: 
Race:: [[Halfling]]
Romance:: 
Servant:: 
Serves:: 
Workplace:: [[Heidelburg Conservatory]]
Worshiper:: 
%%
# `= this.file.name`
---

A `=this.Gender` `=this.Race` from `=this.Home`. Works at the [[Heidelburg Conservatory]].

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
and [[Fausta]]
sort file.name asc
```