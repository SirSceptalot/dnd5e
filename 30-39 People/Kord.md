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
Gender:: male
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
Race:: God
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

Commandments of the Stormlord
- Bravery above all. There is no glory in cowardice.
- Strength is the path to greatness, but greatness is the responsible use of strength.
- The glory of the Stormlord lives through your glory on the battlefield.

Also known as "The Stormlord", this god revels in strength and battlefield prowess. He is revered mostly by warriors and athletes.

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
and [[Kord]]
sort file.name asc
```