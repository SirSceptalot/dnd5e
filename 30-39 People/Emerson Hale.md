---
hide-trail: true
---
# `= this.file.name`
%%
Possible entries: Associate; Birthday; DestroyDate; Destroyed; Enemy; FirstSeenDate; FirstSeenLocation; Gender; Home; Icon; Job; LastLocation; Leads; MemberOf; Offspring; Owns; Parent; Race; Romance; Servant; Serves; Workplace; Worshiper
These values are added below. Fill in known info and delete the rest.
Keep the above list intact so you can insert things in the correct alphabetical order when adding back a field if you obtain new information.
%%
[DestroyDate:: [[0835-10-16]]]
[Destroyed:: Yes]
[FirstSeenLocation:: [[Avelund]]]
[Gender:: male]
[Home:: [[Avelund]]]
[Job:: Guild master]
[LastLocation:: [[Avelund]]]
[Race:: [[Human]]]

---

[[0835-10-12]]:  Arinya sees him sneaking around and uses a spell to communicate with him. He says he's on his way to smash the vials he picked up earlier at the gate. He wants to do it specifically at the gate in order to send a message, although he doesn't want to get caught.

[[0835-10-13]]

[[0835-10-15]]: Emerson turns out to be a traitor to the [[Avelund Resistance]].

[[0835-10-16]]: I execute Emerson to spare him from the death by torture he would surely face if given a public trial.

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
and [[Emerson Hale]]
sort file.name asc
```