# Grand Theft Bike V - Metadata API <!-- omit in toc -->

This document contains the API specification for interfaces that use course metadata.

## HTML Dictionary <!-- omit in toc -->

The html model contains the following element:

### RouteDB  <!-- omit in toc -->

| Column         | Data Type | Description                                               | Example                                         |
| :------------- | :-------- | :-------------------------------------------------------- | :---------------------------------------------- |
| Name           | string    | Name. Note: must match filename without ".json" extension | `road_vinewood_heights`                         |
| Author         | string    | Author                                                    | `Richard Slaughter`                             |
| Map            | string    | Map (link to image of route map)                          | `https://imgur.com/QG89zk1.jpg`                 |
| RouteType      | string    | RouteType (road, gravel, mtb, bmx, mix, etc)              | `Road`                                          |
| Distance (km)  | decimal   | Distance (km)                                             | `8.2`                                           |
| Distance (mi)  | decimal   | Distance (mi)                                             | `5.1`                                           |
| Elevation (m)  | int       | Elevation (m)                                             | `193`                                           |
| Elevation (ft) | int       | Elevation (ft)                                            | `634`                                           |
| Description    | string    | Description                                               | `A hilly zigzag through ritzy Vinewood Heights` |


## Route Metadata Dictionary <!-- omit in toc -->

The metadata model contains the following elements:

- [Route](#route)
- [RouteCategory](#routecategory)
- [RouteDetail](#routedetail)
- [RouteMap](#routemap)
- [RouteMedia](#routemedia)
- [RouteRating](#routerating)
- [RouteSegment](#routesegment)
- [RouteType](#routetype)
- [Waypoint](#waypoint)
- [WaypointConfig](#waypointconfig)

### Route

| Column           | Data Type | Description                | Example |
| :--------------- | :-------- | :------------------------- | :------ |
| RouteID          | string    | route identifier           | `1`     |
| RouteCategoryID  | string    | route category identifier  | `1`     |
| RouteDetailID    | string    | route detail identifier    | `1`     |
| RouteTypeID      | string    | route type identifier      | `1`     |
| WaypointConfigID | string    | waypoint config identifier | `1`     |

### RouteCategory

| Column            | Data Type | Description               | Example                       |
| :---------------- | :-------- | :------------------------ | :---------------------------- |
| RouteCategoryID   | string    | route category identifier | `1`                           |
| RouteCategoryName | string    | route category name       | `BMX`,`Gravel`, `MTB`, `Road` |

### RouteDetail

| Column                 | Data Type | Description             | Example                           |
| :--------------------- | :-------- | :---------------------- | :-------------------------------- |
| RouteDetailID          | string    | route detail identifier | `1`                               |
| RouteDetailAuthor      | string    | route author            | `Matthias Urech`                  |
| RouteDetailDescription | string    | route description       | `Roads in Los Santos harbor area` |
| RouteDetailDistanceKm  | decimal   | route distance (km)     | `17.0`                            |
| RouteDetailDistanceMi  | decimal   | route distance (mi)     | `10.5`                            |
| RouteDetailElevationM  | int       | route elevation (m)     | `190`                             |
| RouteDetailElevationFt | int       | route elevation (ft)    | `623`                             |
| RouteDetailName        | string    | route name              | `Docklands`                       |

### RouteMap

| Column           | Data Type | Description      | Example               |
| :--------------- | :-------- | :--------------- | :-------------------- |
| RouteMapID       | string    | map identifier   | `1`                   |
| RouteMapCounty   | string    | map county       | `Blaine County`       |
| RouteMapLocation | string    | map location     | `Grand Senora Desert` |
| RouteMapName     | string    | map name         | `Sandy Shores`        |
| RouteMapObject   | string    | map object       | `Town`                |
| RouteID          | string    | route identifier | `1`                   |

### RouteMedia

| Column                | Data Type | Description       | Example                                           |
| :-------------------- | :-------- | :---------------- | :------------------------------------------------ |
| RouteMediaID          | string    | media identifier  | `1`                                               |
| RouteMediaDescription | string    | media description | `course preview`                                  |
| RouteMediaFileName    | string    | media file name   | `road_docklands.png`                              |
| RouteMediaFileUrl     | string    | media file url    | `https://github.com/gtbikev/docs/courses/images/` |
| RouteMediaType        | string    | media type        | `map`                                             |
| RouteID               | string    | route identifier  | `1`                                               |

### RouteRating

| Column           | Data Type | Description       | Example              |
| :--------------- | :-------- | :---------------- | :------------------- |
| RouteRatingID    | string    | rating identifier | `1`                  |
| RouteRatingType  | string    | rating type       | `Hilly`              |
| RouteRatingValue | string    | rating value      | `Medium steep climb` |
| RouteID          | string    | route identifier  | `1`                  |

### RouteSegment

| Column                  | Data Type | Description            | Example                |
| :---------------------- | :-------- | :--------------------- | :--------------------- |
| RouteSegmentID          | string    | segment identifier     | `1`                    |
| RouteSegmentDistanceKm  | decimal   | segment distance (km)  | `1.6`                  |
| RouteSegmentDistanceMi  | decimal   | segment distance (mi)  | `1.0`                  |
| RouteSegmentElevationM  | int       | segment elevation (m)  | `100`                  |
| RouteSegmentElevationFt | int       | segment elevation (ft) | `328`                  |
| RouteSegmentGradient    | int       | segment gradient (%)   | `3`                    |
| RouteSegmentName        | string    | segment name           | `not really an uphill` |
| RouteID                 | string    | route identifier       | `1`                    |

### RouteType

| Column           | Data Type | Description     | Example             |
| :--------------- | :-------- | :-------------- | :------------------ |
| RouteTypeID      | string    | type identifier | `1`                 |
| RouteTypeName    | string    | type name       | `Mixed`             |
| RouteTypeSurface | string    | type surface    | `Gravel & Hardpack` |

### Waypoint

| Column            | Data Type | Description         | Example   |
| :---------------- | :-------- | :------------------ | :-------- |
| WaypointID        | string    | waypoint identifier | `1`       |
| WaypointPositionX | decimal   | waypoint position x | `-1587.1` |
| WaypointPositionY | decimal   | waypoint position y | `4756.2`  |
| WaypointPositionZ | decimal   | waypoint position z | `50.9`    |
| WaypointRotationX | decimal   | waypoint rotation x | `0.0`     |
| WaypointRotationY | decimal   | waypoint rotation y | `0.0`     |
| WaypointRotationZ | decimal   | waypoint rotation z | `0.0`     |
| RouteID           | string    | route identifier    | `1`       |

### WaypointConfig

| Column               | Data Type | Description                              | Example    |
| :------------------- | :-------- | :--------------------------------------- | :--------- |
| WaypointConfigID     | string    | waypoint config identifier               | `1`        |
| WaypointConfigColor  | string    | waypoint default color (html color code) | `FFADFF2F` |
| WaypointConfigRadius | decimal   | waypoint default radius                  | `10.0`     |
