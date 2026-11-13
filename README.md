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
| `shoreline-full` | GSHHG 2.3.7 shoreline with its full resolution, P. Wessel and W. H. F. Smith | LGPL-3.0-or-later |
| `geoid-egm2008-fine` | EGM2008 geoid at 2.5′ (NGA, via PROJ), replacing the base pack's 5′ grid | Public domain (NGA) |
| `geoid-osgm15` | OSGM15 geoid for Ordnance Datum Newlyn, Great Britain (Ordnance Survey, via PROJ) | BSD-2-Clause |

Each pack carries its licence notices in `licences/`.
