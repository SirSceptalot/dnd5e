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
Race:: creature
Romance:: 
Servant:: 
Serves:: 
Workplace:: 
Worshiper:: 
%%
# `= this.file.name`
---

Commandments of the Platinum Dragon
- Stand as a paragon of honour and justice.
- Smite evil wherever it is found, yet show compassion to those who have strayed from righteousness.
- Defend the weak, bring freedom to those without, and protect the ideals of just order.

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
and [[Bahamut]]
sort file.name asc
```