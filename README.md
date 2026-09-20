# South King Link Light Rail Corridor Map

A historical ArcGIS Pro map of Link light rail stations and rail-segment status from Tukwila International Boulevard Station to Federal Way Downtown Station, using data dated **January 31, 2025**.

## Purpose

I created this map to compare the mapped in-service and under-construction status of stations and rail segments in the selected South King corridor in one readable layout.

## Data and attribution

The map uses `LINKLine`, `LINKStations`, and `STSubareas` from the [Sound Transit Open Transit Data portal](https://www.soundtransit.org/). The source geodatabase and ArcGIS project are not included. Obtain authorized layers from the official portal and review current attribution, disclaimer, publication-status, and licensing terms before reuse.

The map date is January 31, 2025. Source metadata reports a different extract date; these dates are not interchangeable. This map is not an official Sound Transit publication or a live service/construction feed.

## Workflow and design

I selected the Link rail, station, and subarea layers, filtered the display to the South King corridor, and used blue for **In Service** and amber for **Under Construction**. Labels, subarea context, legend, scale bar, north arrow, and source credits complete the layout.

![South King Link light rail corridor map](map.jpg)

*Historical corridor map showing station and rail-segment status as of January 31, 2025.*

## Interpretation and limitations

Angle Lake and the stations north of it were shown as in service. Kent Des Moines, Star Lake, Federal Way Downtown, and the southern rail segment were shown as under construction. The map communicates location and mapped status; it does not measure completion, predict opening dates, or evaluate ridership.

Verify current Sound Transit information before travel or project decisions. The selected corridor simplifies the regional network, and subarea boundaries provide context rather than service coverage.

## Reproducibility

In ArcGIS Pro, obtain authorized copies of the cited layers, filter the corridor and status fields, apply the documented colors, compose the layout, and export the image. Exact regeneration requires confirmed source permissions and extraction metadata.

## Repository contents

- `map.jpg` — exported map
- `README.md` — data, design, interpretation, and reuse boundary
