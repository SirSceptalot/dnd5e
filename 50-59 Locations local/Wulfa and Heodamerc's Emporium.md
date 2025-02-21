%%
ParentPage:: [[Avelund]]
LocationType:: [[Address]]

ParentPage is the geographic container that this location is in.
LocationType can be one of the following: Planet, Continent, Nation, Area, City, District, Address. This value must be defined as a page link within double quotes.
%%
# `= this.file.name`
```leaflet
id: avelund
image: [[Avelund.png]]
minZoom: 5
maxZoom: 10
defaultZoom: 6.3
zoomDelta: 0.1
unit: meter
scale: 500
```
Magic shop in [[Avelund]]. We raided this with permission of city officials in order to acquire materials to fight the [[Exaltators]].

Visited on: 
```dataview
list
from [[Wulfa and Heodamerc's Emporium]]
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