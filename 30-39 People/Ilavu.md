---
hide-trail: true
---

FirstSeenDate:: [[0835-09-12]]
FirstSeenLocation:: the material plane
Gender:: male
Job:: Giant Speaker
MemberOf:: [[StormMaw Tribe]]
Race:: [[Goliath]]

---

A `=this.Gender` `=this.Race` from the [[StormMaw Tribe]] that currently holds the title "`=this.Job`"
He communicates with a [[Storm Giant]] that produces whiskey for the tribe, which they then distribute to others.

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
and [[Ilavu]]
sort file.name asc
```