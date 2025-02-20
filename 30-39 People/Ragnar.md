#race/variant-human/obsidian 

An obsidian loyal to House Telemanus, he was killed defending the city of Tinos from the forces of the Ashlord in front of a young [[Pax au Telemanus]].

He was an Obsidian of exceptional size, strength and ability, easily outclassing Golds and some Peerless Scarred with minimal effort.

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
and [[Ragnar]]
sort file.name asc
```