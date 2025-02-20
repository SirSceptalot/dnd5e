---
hide-trail: true
---
# `= this.file.name`
[Birthday:: ]
[DestroyDate:: ]
[Destroyed:: No]
[Enemy:: ]
[FirstSeenLocation:: [[Collegento]]]
[Gender:: female]
[Home:: [[Collegento]]]
[Icon:: [[Pelor]]]
[Job:: Cleric]
[LastLocation:: ]
[Leader:: ]
[Leads:: ]
[MemberOf:: [[The Experts]]]
[Offspring:: ]
[Owns:: ]
[Parent:: ]
[Race:: [[Human]]]
[Romance:: ]
[Servant:: ]
[Serves:: ]
[Workplace:: ]
[Worshiper:: ]

---

[[0835-09-07]]: [[Camedyr Baughan]] tells us that this was a human female cleric, living in [[Ashein]] of [[Pelor]] that somehow fractured her own soul to obtain magic normally out of mortal reach to stop the [[Skogsland]] army from advancing any further.

She succeeded, but not only destroyed the advancing enemy (from her perspective) army, but also her own life, soul, and the lives of countless residents.

Her soul is supposedly locked in a gem there.

[[0835-09-20 (continued)]]: we return from the Far Realms with three soul shards containing another portion of her soul.

[[Tiziano]] manages to communicate with her soul through the soul shards, and discovers that she had traded her soul with the entity known as [[The Gatekeeper]], in return for powers that let her stop Skogsland's advancing army.

Later that day, we free her soul from the torture rock it was contained in, and take it with us (with her own consent).

[[0835-09-21]]: Nivemera agrees to become part of our team.

[[0835-09-27]]: We leave her soul with my friend [[Balthazar Gelt]] so he can fabricate a safer container for her.

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
and [[Nivemera]]
sort file.name asc
```