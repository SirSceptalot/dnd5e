---
hide-trail: true
---
# `= this.file.name`

[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: ]
[Gender:: female]
[Home:: the Nine Hells]
[Icon:: ]
[Job:: deity]
[Leads:: Evil Chromatic Dragons]
[MemberOf:: "The Pantheon of the Dragon"]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: Dragon]
[Romance:: ]
[Servant:: ]
[Serves:: Herself]
[Workplace:: The Nine Hells]

---

Tiamat is a powerful, five-headed dragon deity who represents the evil chromatic dragons. She is often depicted as a dragon with one head for each color of the chromatic dragons: red, green, blue, black, and white. Tiamat is believed to be one of the oldest deities in the pantheon and is revered by many evil dragons and dragonborn as the mother of all dragonkind. Tiamat is typically portrayed as being greedy, power-hungry, and cruel, and she is known to demand tribute and sacrifices from her followers. She is currently in the first circle of hell.


Allies:
```dataview
list FROM "30 Characters"
WHERE any(contains(MemberOf, this.MemberOf))
AND MemberOf != NULL
AND file.name != this.file.name
sort file.name asc
```

```dataview
table without id file.link as "Sighting/Interaction", Location
from "10 Journal"
and [[Tiamat]]
sort file.name asc
```