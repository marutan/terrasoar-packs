# Terra Soar data packs

Extra data packs for [Terra Soar](https://github.com/marutan/terrasoar),
installed from the application with **File > Data Packs…**.

- `index.json` lists the packs. The application reads it from this
  repository's main branch.
- Each pack version is a release named `<pack id>-<version>`, with the
  pack's manifest and files attached.

The packs are built from pinned sources by Terra Soar's packager
(`make packs`; see `docs/tools/packager.md` there), which also writes each
pack's entry for `index.json`. Index format and install process:
`docs/design/packs.md`.

| Pack | What | Licence |
| --- | --- | --- |
| `bluemarble-full` | NASA Blue Marble (July 2004, topography and bathymetry) at full resolution | Public domain (NASA) |
| `bluemarble-monthly` | NASA Blue Marble for each month of 2004 (5400 × 2700 px each), variants the Blue Marble layer picks by the program's clock | Public domain (NASA) |
| `shoreline-full` | GSHHG 2.3.7 shoreline with its full resolution, P. Wessel and W. H. F. Smith | LGPL-3.0-or-later |
| `geoid-egm2008-fine` | EGM2008 geoid at 2.5′ (NGA, via PROJ), replacing the base pack's 5′ grid | Public domain (NGA) |
| `geoid-osgm15` | UK grids: OSGM15 geoid for Ordnance Datum Newlyn and OSTN15 (OSGB36 to ETRS89), Great Britain (Ordnance Survey, via PROJ) | BSD-2-Clause |
| `vmap0-boundaries` | NGA Vector Map Level 0 (VMAP0, 1:1,000,000, edition 5, 2000): international and disputed boundaries, claim lines, the Date Line | Public domain (NGA) |
| `vmap0-transportation` | VMAP0: roads, railways, trails, ferry routes, bridges, tunnels and airports | Public domain (NGA) |
| `vmap0-population` | VMAP0: built-up areas, named settlements (labels) and landmarks | Public domain (NGA) |
| `vmap0-other` | VMAP0: ice, sand and lava fields, mines, quarries, oil fields, plants, storage, pipelines and power lines | Public domain (NGA) |
| `vmap0-hydrography-noamer`, `-eurnasia`, `-soamafr`, `-sasaus` | VMAP0: rivers, lakes, canals, dams and coastlines, one pack per VMAP0 library (North America; Europe and North Asia; South America, Africa and Antarctica; South Asia and Australia) | Public domain (NGA) |
| `vmap0-elevation-noamer`, `-eurnasia`, `-soamafr`, `-sasaus` | VMAP0: contours, spot heights and depth contours, one pack per library | Public domain (NGA) |
| `vmap0-vegetation-noamer`, `-eurnasia`, `-soamafr`, `-sasaus` | VMAP0: woodland, cropland, grassland and scrub, marsh and swamp, and tundra, one pack per library | Public domain (NGA) |
| `vmap0-admin` | VMAP0's first-order administrative boundaries (states, provinces) and named administrative areas, which are ESRI's, kept apart from the public-domain packs | ESRI Data License Agreement (internal or non-commercial use only) |
| `naturalearth-10m` | Natural Earth 1:10m map layers: rivers, lakes, places, roads, railways, airports, ports, time zones, state borders, peaks | Public domain (Natural Earth) |
| `naturalearth-relief`, `-hypsometric`, `-shaded-relief` | Natural Earth's 1:10m raster maps: Natural Earth I, cross-blended hypsometric tints, grey shaded relief | Public domain (Natural Earth) |
| `blackmarble` | NASA Black Marble, the Earth at night, 2012 and 2016 at 3 km | Public domain (NASA) |
| `wdbii` | WDBII borders, rivers and canals from GSHHG 2.3.7, P. Wessel and W. H. F. Smith | LGPL-3.0-or-later |
| `ourairports` | OurAirports airports, runways and navigation aids, 2026-11-22 | Public domain (Unlicense) |
| `names` | Place and feature names: NGA GNS outside the US, USGS GNIS in it | Public domain (US government works) |
| `elevation-etopo-30s` | ETOPO 2022 at 30″, replacing the base pack's terrain | CC0-1.0 (NOAA) |
| `gebco-w180-w90`, `-w90-0`, `-0-e90`, `-e90-e180` | The GEBCO 2026 Grid at 15″ (land and sea floor), one pack per quarter of the world, read together as one layer | Public domain (GEBCO) |

Each pack carries its licence notices in `licences/`. The raw sources of
every pack, with their licences, are kept in
[marutan/terrasoar-packs-sources](https://github.com/marutan/terrasoar-packs-sources).
