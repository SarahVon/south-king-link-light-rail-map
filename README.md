# South King Link Light Rail Corridor Map

A historical ArcGIS Pro map of Link light rail stations and rail-segment status from Tukwila International Boulevard Station to Federal Way Downtown Station, using data dated **January 31, 2025**.

## Contents

- [Purpose and questions](#purpose-and-questions)
- [Data and source boundary](#data-and-source-boundary)
- [Workflow and design](#workflow-and-design)
- [Map](#map)
- [Interpretation](#interpretation)
- [Limitations](#limitations)
- [Reproducibility and attribution](#reproducibility-and-attribution)
- [Repository contents](#repository-contents)

## Purpose and questions

The map asks: **Which stations and rail segments in the selected South King corridor were mapped as in service or under construction on January 31, 2025, and how can that status be read quickly in one layout?**

## Data and source boundary

The source layers came from the Sound Transit Open Transit Data portal: `LINKLine` for rail alignments and status, `LINKStations` for station locations and status, and `STSubareas` for geographic context. The repository contains the exported map, not the source geodatabase or ArcGIS project. Status is a historical attribute snapshot, not a live construction or service feed.

## Workflow and design

1. Selected the Link rail, station, and subarea layers from the broader transit data.
2. Filtered the display to the South King corridor and the depicted extent.
3. Used blue for features mapped as **In Service** and amber for **Under Construction**, with matching station and line colors.
4. Added translucent subarea context, station labels, legend, scale bar, north arrow, and source credits. The visible subareas are East King, North King, Pierce, and South King; Snohomish was outside the displayed extent.

## Map

![South King Link light rail corridor map](map.jpg)

*Historical corridor map showing station and rail-segment status as of January 31, 2025.*

## Interpretation

Angle Lake and the stations to its north on the depicted line were shown as in service. Kent Des Moines, Star Lake, and Federal Way Downtown, along with the southern rail segment, were shown as under construction. The layout communicates location and mapped status; it does not measure construction completion, predict opening dates, or evaluate ridership or project performance.

## Limitations

This is a historical map, not a Sound Transit publication or current service guide. Verify current Sound Transit information before travel or project decisions. The selected corridor simplifies the regional network, and subarea boundaries provide context rather than a measure of service coverage. Station names and labels should be checked against original dataset records when an authoritative historical record is required.

## Reproducibility and attribution

Recreate the map in ArcGIS Pro by obtaining the cited Sound Transit layers, filtering the corridor and status fields, applying the documented colors, composing the layout elements, and exporting the image. Exact regeneration is bounded because the source data, project file, and extraction metadata are not included. Basemap and map credits appear on the exported layout. Check current portal terms and dataset metadata before reuse.

## Repository contents

- `map.jpg` — exported final map
- `README.md` — data, design, interpretation, and reuse boundary
