# MUSA6950-AI-for-Urban-Sustainability
Final Project for AI for Urban Sustainability

## Research question:
The final project seeks to answer the question: Which direction would lava flow in a volcanic eruption? By measuring the lava flow, we can see which communities living near volcanoes are at higher risk. This could inform emergency services, which communities should be evacuated first. The volcanoes studied are from Indonesia. Indonesia is selected because of its large number of active volcanoes, at 59.

## Methodology
The coordinates of active volcanoes from Indonesia are taken from the [Smithsonian Institution, 2025](https://volcano.si.edu/). I define active volcanoes as those with last eruptions since 1900. The list of volcanoes and their coordinates are in Appendix 1.
Digital Elevation Model (DEM) tiles are downloaded from [NASADEM HGT v001on Microsoft Planetary Computer](https://planetarycomputer.microsoft.com/dataset/nasadem). NASADEM provides global topographic data at 1 arc-second (~30m) horizontal resolution, derived primarily from data captured via the Shuttle Radar Topography Mission (NASA, 2025).
I use flood mapping techniques from [PyFlwDir (Deltares, 2025)](https://deltares.github.io/pyflwdir/latest/index.html). PyFlwDir is created by Deltares, an “independent research institute for applied research in the field of water and subsoil based in Delft”, the Netherlands (Deltares, 2025). The techniques applied are 1) Flow directions from elevation data, 2) Tracing flow directions, and 3) Height Above Nearest Drainage (HAND).

I first calculate the flow direction from the elevation data. I then trace the flow directions. Finally, I calculated the HAND for each tile
