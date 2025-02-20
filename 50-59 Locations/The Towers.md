%%
ParentPage:: [[Amaroth]]
LocationType:: [[District]]

ParentPage is the geographic container that this location is in.
LocationType can be one of the following: Planet, Continent, Nation, Area, City, District, Address. This value must be defined as a page link within double quotes.
%%
# `= this.file.name`

```leaflet
id: Amaroth-thetowers
image: [[Amaroth.png]]
minZoom: 6
maxZoom: 10
defaultZoom: 7.5
zoomDelta: 0.5
lat: 67.5
long: 60
unit: meter
scale: 297
```

All the wizards of [[Amaroth]] have their towers here, all trying to outdo one another in their splendor and grandeur.

Visited on: 
```dataview
list
from [[The Towers]]
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