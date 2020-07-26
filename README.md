# libProteus geographical water body data

A repository of geographical water body data, used directly by the libProteus GeoInfo subsystem.

The data contained here are processed from the ASTER Global Water Bodies Database (ASTWBD) Version 1 data (https://cmr.earthdata.nasa.gov/search/concepts/C1575734433-LPDAAC_ECS.html), with the primary goal of reducing the amount of storage space required.

Each data file is a gzip-compressed bit field, indicating the presence of land or water within a particular geographical "square degree", with 1-arcsecond resolution (3600x3600 bits in each "square degree" tile). Tiles which are not present (based on file name) are assumed to consist entirely of water.
