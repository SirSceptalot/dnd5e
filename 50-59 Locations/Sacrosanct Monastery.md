---
aliases: [Monestary of Saint Solar Macharius]
---
%%
ParentPage:: 
LocationType:: [[Address]]

ParentPage is the geographic container that this location is in.
LocationType can be one of the following: Planet, Continent, Nation, Area, City, District, Address. This value must be defined as a page link within double quotes.
%%
# `= this.file.name`
```leaflet
id: midlands
image: [[Midlands.png]]
minZoom: 5
maxZoom: 10
defaultZoom: 6.3
zoomDelta: 0.1
unit: meter
scale: 500
```
Description

sacrosanct monestary (correcte spelling) trekt zich niets aan van de rest van de wereld, ze kijken enkel om hun eigen missie: zorgen dat er niets uit aurocondor vertrekt
het is en een orde gesticht door de heilige macharius, waardoor ze redelijk strikt zijn
enkel de besten kunnen toetreden, en het is een hele eer om te kunnen toedreden
verschillende palladin ordes van ashein vinden het een fucking big deal om mensen te mogen sturen
qua supplies zijn ze redelijk afhankelijk van ashein, maar ze hebben genoeg clerics die met magie kunnen voor proviand zorgen
alles lijkt te wijzen naar een strikte paladin religieuze orde, maar niet gedediceert aan 1 god, maar verschillende. Mostly: keep the darkness at bay kind of people
als aurocondor opgeslokt werd waren zijn de enigen die nog iets of iemand er IN sturen, maar niet er uit. Er UIT raken konden ze niets aan doen, maar sommige wezens zijn sterk genoeg en ze konden het zelf

wanneer aurocondor gerrezen is zijn zij de enigen die een barriere kunnen maken om te zorgen dat er niets UIT aurocondor gaat


Visited on: 
```dataview
list
from [[Sacrosanct Monastery]]
and "10 Journal"
sort file.name asc
```

```dataview
table without id rows.file.link as Resident, Home, rows.Job as Job
from "30 Characters"
where Home = this.file.name
or Home = this.file.link
or contains(Home.ParentPage, this.file.link)
sort Home asc, file.link asc, Job asc
group by Home
```

```dataview
table without id file.link as "Sub location", LocationType as Type
from "50 Locations"
where ParentPage = this.file.link
or ParentPage.ParentPage = this.file.link
or ParentPage.ParentPage.ParentPage = this.file.link
or ParentPage.ParentPage.ParentPage.ParentPage = this.file.link
or ParentPage.ParentPage.ParentPage.ParentPage.ParentPage = this.file.link
or ParentPage.ParentPage.ParentPage.ParentPage.ParentPage.ParentPage = this.file.link
sort file.link.LocationType.LocationLevel asc, file.name asc
```