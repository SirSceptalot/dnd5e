---
hide-trail: true
aliases: [Weezard]
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
Gender:: male
Home:: [[The Towers]]
Icon:: 
Job:: Wizard
LastLocation:: 
Leader:: 
Leads:: 
MemberOf:: 
Offspring:: 
Owns:: 
Parent:: 
Race:: [[Human]]
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

Balthazar "WEEzard" Gelt, one of my oldest friends and one of the first humans I saw after my creation.

He specialises in metallurgy.

His Tower is made of (what looks like) pure gold.

[[0835-09-27]]: We visit Weezard to ask if he can fabricate a medallion to house the soul of [[Nivemera]]

[[0836-03-26]]: We call upon him once again to ask if he can perform my [[Leg upgrade]].
He has transformed himself to be made entirely of gold.

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
and [[Balthazar Gelt]]
sort file.name asc
```