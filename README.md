# Green Shores eligibility plots

An interactive map of the plots surveyed for Green Shores eligibility in Madagascar, with the field photos for each plot.

**[Open the map](https://aebwwfdk.github.io/gs-eligibility-map/)**

It works in any modern browser on desktop or phone. An internet connection is needed for the basemap.

## What you can do

- **Select a plot** to see its area in hectares, restoration difficulty, eligibility, field photos and survey notes. Select a photo to enlarge it, and use the arrow keys to move between photos.
- **Colour the plots** by site, restoration difficulty, natural regeneration, regeneration pattern, number of barriers to regeneration, number of recommended interventions, or yes/no questions such as agriculture and threats. The legend shows the number of plots and hectares in each category. Select a category to hide or show it.
- **Filter the plots** by site, operator, restoration difficulty, eligibility, barrier to regeneration or recommended intervention.
- **Find a plot** by typing its ID.
- **Compare sites** with a chart showing how each site's plots split across a category, by hectares or by number of plots. Select a site in the chart to filter the map to it.
- **Switch layers on and off**, including the CBO names and the planting shortlist, and change the basemap between satellite, streets and light grey.

## Reading the map

| Layer | How it looks | What it shows |
| --- | --- | --- |
| CBO boundaries | Coloured outlines with names. Dashed outlines mark CBOs that are not yet official. | The areas of the VELUX CBOs |
| Eligibility plots | Filled polygons, coloured by the option chosen under "Colour plots by" | The plots surveyed in the field |
| Planting shortlist | Bright pink outline with a white halo | Areas shortlisted for planting, ranked overall and within each CBO |

## About the data

- **Plots.** The plots were identified by the consultancy Biotope and visited by several operators between June and August 2026. Area is shown in hectares.
- **Plot IDs.** IDs follow the pattern `MG2055_SITE_RA_n`. Each operator numbered their plots from 1 within a site, so the same ID can belong to several plots in different places. The "Find a plot" list adds the operator and visit date to tell them apart.
- **Photos.** Photos are placed on plots by their GPS location. Some photos were filed under another plot's label, and these were placed on the plot they were taken in. Two photos taken 90 to 100 m from the nearest plot were assigned to that nearest plot.
- **Questions asked only where there is regeneration.** The regeneration pattern and threat questions were only answered for plots with some natural regeneration. The other plots show as "No data" in those colour options.
- **Planting shortlist.** The shortlist has its own polygons and is not linked to individual plots. Photos are attached to the eligibility plots only.
- **Coded values.** Survey codes such as `antr_threats` are shown as readable labels.

## Good to know

- The map is a snapshot. The date of the last export is shown at the bottom of the control panel.
- The site is public. Anyone with the link can view the map, and the plot data and photos can be downloaded from this repository.

## Updating the map

1. In the ArcGIS Pro project, run the map build script. It writes `index.html` and the `photos` and `thumbs` folders.
2. In the repository folder, delete the old `photos` and `thumbs` folders, then copy in the new `index.html`, `photos` and `thumbs`.
3. In GitHub Desktop, commit the changes and select **Push origin**. The site refreshes a minute or two later at the same link.

## Credits

Basemaps: Esri World Imagery, OpenStreetMap contributors, and CARTO. The map is built with [Leaflet](https://leafletjs.com).

Questions or corrections? Contact the Green Shores team at WWF Denmark.
