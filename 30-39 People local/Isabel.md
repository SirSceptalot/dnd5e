---
aliases: 
---

Ally:: [[Ephemera]]
FirstSeenDate:: [[0835-09-02]]
FirstSeenLocation:: [[Mercenary Ring]]
Gender:: female
Home:: [[Lawold]]
LastLocation:: [[Lawold]]
Race:: [[Human]]


Slave girl held captive in a brothel named the [[Swift Finish]].
After we rescued her, she accepted our offer to tag along to Ephemera's home.

Along the way there we passed close to her home in [[Lawold]] on [[0835-09-04]], and she went the rest of the way on her own.


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
and [[Isabel]]
sort file.name asc
```