# CCVA Flood Tiles
Raster tile pyramids for the Climate Change Vulnerability Assessment Tool —
localized flood screening layers for the Twin Cities 7-county metro region.

## Layers

### Flood impact zones, 2026 (current) — `flood_2026/`
Source: Met Council bluespot screening rerun on the MN DNR MnTopo 1 m DEM
(2021–23), same method and classes as the 2011 layer.
Classes: Primary (highest risk) → Secondary → Tertiary → Shallow
Unpacked byte for byte from `flood_2026.pmtiles` (the app's map layer) by
ccva-data `scripts/unpack_flood_2026_xyz.py`; used by the app's PDF report.

https://metropolitan-council.github.io/ccva-tiles-flood/flood_2026/{z}/{x}/{y}.png

### Localized Flood Screening, 2011 (retired) — `flood/`
Source: Met Council Localized Flood Screening, LiDAR-derived bluespots (2011).
No longer used by the app as of 2026-11-20; kept so the 2011 layer can be restored.

https://metropolitan-council.github.io/ccva-tiles-flood/flood/{z}/{x}/{y}.png

## Usage
Zoom range: 9–16 | CRS: EPSG:3857
