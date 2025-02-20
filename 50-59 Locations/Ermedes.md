%%
ParentPage:: [[Midlands]]
LocationType:: [[City]]

ParentPage is the geographic container that this location is in.
LocationType can be one of the following: Planet, Continent, Nation, Area, City, District, Address. This value must be defined as a page link within double quotes.
%%
# `= this.file.name`
```leaflet
id: ermedes
image: [[Ermedes.png]]
minZoom: 5
maxZoom: 10
defaultZoom: 6.4
zoomDelta: 0.1
unit: meter
scale: 172
height: 760px
```

This city once belonged to [[Ashein]], but has been given up at the end of the war in order to serve as a buffer state between [[Ashein]] and [[Skogsland]].
It now has the status of city-state.


Visited on: 
```dataview
list
from [[Ermedes]]
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