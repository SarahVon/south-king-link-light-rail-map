# South King Link Light Rail Corridor Map

A historical ArcGIS Pro map of Link light rail stations and rail-segment status from Tukwila International Boulevard Station to Federal Way Downtown Station, using data dated January 31, 2025.

## Methods and design

- Selected Link rail alignments, stations, and Sound Transit subarea boundaries from the Sound Transit Open Transit Data portal.
- Focused the extent on the South King corridor for legibility.
- Used blue for features mapped as **In Service** and amber for features mapped as **Under Construction**.
- Added station labels, a legend, scale bar, north arrow, and translucent subarea context.

## Output

- `map.jpg` — exported final map.

## Visualization

![South King Link light rail corridor map](map.jpg)

*Historical corridor map showing station and rail-segment status as of January 31, 2025.*

## Limitations

This is an academic visualization and historical snapshot, not a Sound Transit publication or current service guide. Statuses reflect the source data and stated date; verify current Sound Transit information before using the map for travel or project decisions. The selected corridor simplifies the regional network, and subarea boundaries are contextual rather than a measure of service coverage. Station names and labels should be checked against the original dataset records if an authoritative historical record is required.

## Attribution

Tool: ArcGIS Pro. Transit source: Sound Transit Open Transit Data portal, including `LINKLine`, `LINKStations`, and `STSubareas` layers. **Attribution placeholder:** confirm the portal URL, dataset version, basemap credits, and license language before publication.

Author: Sarah Anderson. Context: university GIS coursework, revised for portfolio presentation.
