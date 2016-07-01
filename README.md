# tmdl-grass-swale-map
Map of TMDL grass swales for access on mobile devices.

### Conversion

Instructions are WIP, but basically using Esri2Open

### Data Cleanup

1. Prettify the geoJSON output.
2. Find and replace the following regex with `null` using Atom

     ^(.*"Category"|.*Long|.*Swale|.*flowl|.*shape|.*Class|.*median|.*totseg|.*index_|.*slope|.*Categorynm|.*fid).*$

3. Replace any instance of `marker_` with `marker-`
4. Prettify again
5. Replace the [swales geoJSON](data\swales.geojson) with the new data.
