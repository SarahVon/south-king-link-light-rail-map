# South King County Link Light Rail Service and Construction Status

This ArcGIS Pro project maps the service and construction status of Link light rail stations and rail segments between Tukwila International Boulevard and Federal Way Downtown. The map provides a focused view of the South King County corridor as it was represented on **January 31, 2025**, distinguishing infrastructure already in service from the Federal Way Link Extension then under construction.

I created the project to practice selecting relevant public data, narrowing a regional dataset to a specific study area, applying status-based symbology, and designing a map that communicates transit expansion clearly.

## Project goals

- Show the location and status of Link stations in the selected South King County corridor.
- Distinguish rail segments that were in service from those under construction.
- Provide regional context with Sound Transit subarea boundaries.
- Create a focused, readable layout from a larger regional transit dataset.

## Final map

![South King County Link light rail service and construction status as of January 2025](map.jpg)

*Historical map of Link light rail service and construction status from Tukwila International Boulevard Station to Federal Way Downtown Station as represented on January 31, 2025.*

## Data

The project uses three GIS layers from Sound Transit's **Open Transit Data** program. Sound Transit describes the portal as a source of publicly accessible transit data for the Puget Sound region.

| Dataset | Geometry | Description | Use in this project |
| --- | --- | --- | --- |
| `LINKLine` | Polyline | Existing and under-construction Link light rail alignments | Mapped rail segments by service or construction status |
| `LINKStations` | Point | Existing and under-construction Link stations | Located and labeled stations by status |
| `STSubareas` | Polygon | Sound Transit subarea boundaries | Provided geographic context for South King and adjacent subareas |

- [Sound Transit Open Transit Data](https://www.soundtransit.org/help-contacts/business-information/open-transit-data-otd)
- [Download current GIS data](https://www.soundtransit.org/help-contacts/business-information/open-transit-data-otd/otd-downloads)
- [Transit Data Terms of Use](https://www.soundtransit.org/help-contacts/business-information/open-transit-data-otd/transit-data-terms-use)

The source files are not redistributed in this repository. Because the portal data can change as projects and service evolve, the official download page is the best source for current files. The map remains a historical representation of the data and project status used for the January 2025 analysis.

## Tools and methods

I completed the project in **ArcGIS Pro** using the following techniques:

- Layer selection and study-area definition
- Attribute review and status-based categorization
- Definition queries and display filtering
- Graduated visual hierarchy and custom symbology
- Station labeling and label placement
- Subarea transparency and contextual mapping
- Layout composition, legend design, and map export

## Workflow

### 1. Define the study area

The source data covers the broader Sound Transit system, so I limited the map to the Link corridor from Tukwila International Boulevard Station south to Federal Way Downtown Station. Removing unrelated routes and stations kept the analysis focused on the South King County expansion and reduced visual clutter.

### 2. Classify stations and rail segments

I reviewed the status attributes in the station and rail-alignment layers and grouped features into two categories: **In Service** and **Under Construction**. The map uses blue for infrastructure shown as operational and amber for infrastructure shown as under construction.

### 3. Add regional context

I included the Sound Transit subareas as semi-transparent polygons. South King provides the primary geographic context, while nearby subareas help orient the corridor within the regional transit district without overpowering the station and alignment data.

### 4. Design the final layout

I labeled each station and organized the legend by station status, rail-alignment status, and subarea. A title, scale bar, north arrow, source note, and preparation date complete the layout. The final design prioritizes the corridor itself while retaining enough surrounding geography to make the station locations understandable.

## Map interpretation

As represented in the January 2025 source data:

- Tukwila International Boulevard, SeaTac/Airport, and Angle Lake stations were shown as **in service**.
- Kent Des Moines, Star Lake, and Federal Way Downtown stations were shown as **under construction**.
- The rail alignment north of Angle Lake was shown as **in service**.
- The extension from Angle Lake toward Federal Way was shown as **under construction**.

Together, the station and alignment layers show how the operating system connected to the southern extension then being developed. The map is intended to communicate location and categorical project status; it does not measure construction progress, predict opening dates, or evaluate ridership or service performance.

## Limitations

This is a historical map rather than a live transit or construction-status product. Station names, service status, project milestones, and source attributes may have changed since January 31, 2025. Current travel or project decisions should be based on official Sound Transit service information.

The selected extent also simplifies the larger regional system. Subarea boundaries provide administrative and geographic context; they do not represent station service areas or rider catchments.

## Repository contents

```text
map.jpg     Final exported map
README.md   Project overview, data documentation, workflow, and interpretation
```

The ArcGIS Pro project and source GIS files are not required to view the completed work. To reproduce or update the map, download the current GIS package from Sound Transit, review the applicable terms, and apply the workflow documented above.

## Attribution

Transit data: Sound Transit Open Transit Data. Basemap credits shown on the map include Esri, Washington State Parks GIS, TomTom, Garmin, SafeGraph, EPA, USFWS, King County, and NOAA.

This independent portfolio project is not an official Sound Transit or WSDOT publication.
