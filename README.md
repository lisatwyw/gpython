# ```gpython```: Python for analyses of **g**eospatial data 

[Site under construction]
 
## Lisa's examples

- [Colab notebook on ```folium```, etc.](https://colab.research.google.com/drive/1hZ4hqzQ9DbEQ_-x4Lou6JcVR5y2My7Mw)
- [Colab notebook on ```osmnx``` package](https://colab.research.google.com/drive/1GsNH-DndcHQUUadXiH-h9v0pDhnxa-Au#scrollTo=8JqN-ftgDDOS)
- [App leveraging ```rasterio```](https://can-ale.streamlit.app/)
- [App demonstrating geocoding and geographic mapping](https://apr5-demo-app1.streamlit.app/)
 
## Popular packages

List compiled and last checked in May 2024:
- [osmnx](https://github.com/gboeing/osmnx-examples/tree/main/notebooks)
- ```geopy```: geolocation; allows users to query geocoordinates by name, addresses of landmarks 
- RSGISLib: remote Sensing and GIS Software Library for Python
- Rtree: Spatial indexing for Python for quick spatial lookups
- [Shapely](https://shapely.readthedocs.io/en/stable/)
- ...

 
<details>

<summary>Geo Datasets</summary>

## Terrain Resource Information Management Program (TRIM 2020), via SFU library

Terrain Resource Information Management Program

> Depending on the region selected, TRIM data may contain the following. Generally, TRIM data comes in two parts for each BCGS region. 1. Digital Elevation Model (DEM). Shapefiles containing elevation points and breaklines. 2. TRIM Positional. Map annotation containing various layers, as listed below. Not all mapsheets contain all layers.
TRIM Contour Annotation Contour annotation for TRIM mapping. Contour text and spot heights. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
>
> TRIM contour lines Index contours (indefinite-depression and combination) and intermediate contour (indefinite-depression and combination), areas of exclusion and Indefinite contours and cliffs. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20, 000.
TRIM Contours Points Contour points, spot heights and mountain peaks. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20,000.
>
> TRIM Cultural Annotation Cultural man made features and landmark text. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20, 000.
>
> TRIM Cultural Lines Cultural man made features - yard, auto wrecker, lumber yard, stock yard (livestock), fish hatchery, electrical substation complex, mines, raw material pile, pit, etc. (see http://srmwww.gov.bc.ca/gis/trimfeatures.htm for full list). The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20,000.
>
> TRIM Cultural Points Cultural point features - barn, silo, greenhouse, station (communication), college, school, university, fire lookout tower, customs office, fire station etc. (see http://srmwww.gov.bc.ca/gis/trimfeatures.htm for full list). The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20,000.
>
> TRIM Landcover Annotation Landcover -wooded area annotation. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
TRIM Landcover Lines Land cover - lines bounding wooded areas, grassland, nurseries, orchards, vineyards, etc. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
>
> TRIM Landcover Points Landcover points. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
TRIM Miscellaneous Annotation Miscellaneous annotation - all features not in the other themes: photo centres, cutlines, etc.. . The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
TRIM Miscellaneous Lines Miscellaneous lines - all features not in the other themes: cutlines, etc. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
>
> TRIM Miscellaneous Points Miscellaneous points - all features not in the other themes, photo centres, etc.. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
>
> TRIM Transportation Annotation Transportation annotation. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
>
> TRIM Transportation Lines Transportation features such as airfields, ferry route, roads, retaining walls, bridges, rail lines, tunnels, pipelines, transmission lines, etc (see http://srmwww.gov.bc.ca/gis/trimfeatures.htm for full list). The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
>
> TRIM Transportation Points Transportation point features - helipads, railway turntable and tollgate. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
> 
> TRIM Water Annotation Water annotation (e.g. lake and river names, etc.). The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
>
> TRIM Water Lines Water features - rivers, lakes, canals, marshes, swamps, reservoirs, falls, rapids, dams, dykes, glaciers, sand bars, etc. (see http://srmwww.gov.bc.ca/gis/trimfeatures.htm for full list). The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.
TRIM Water Points Water point features - rapids, falls, dam, inundated flooded land, marsh, swamp, small breakwall/breakwater, sand/gravel bar, flow arrow, arrowhead, island, island(position approximate), water level, sinkhole. The TRIM program produces digital maps, which is a collection of coverages to conform with the BC Geographic System layout. TRIM mapping consists of 7,027 mapsheets covering the province of British Columbia at a scale of 1:20 000.

</details>

## Resources
 
- [Presentation slides by Feng Jan 2024](https://sustainability-gis.readthedocs.io/en/latest/lessons/L4/disaster-management-with-vgi.html)

   <details>
   
   <summary>Notes</summary>
       
        
    - Subthemes   
        - Epidemiology
        - Participation
        - Transport
        - Social science
        - Social geography
        - Health
        - Climate/ environment
           
    - Social media as source of ambient geographic info
        - Citizen observatories for flood, earthquake, forest fires
        - Need for NLP: resolve ambiguity "flood with people"
        - Sentiments analysis to understand topics: e.g. Hurricanes Harvey, Maria, Irma:
         - caution, advice
         - sympathy, support
         - evidence of injury, mortality, missing people, damage infrastructure, etc.
         - request for donation/ volunteering
         - personal update
        - Phases: preparedness, response, impact, recovery  
        
    - Diff levels of spatial precisions
        - City admin districts
        - POI
        - Geotag tweets (geo coordinate)
       
       
   </details>



## Deep learning & GIS

Huang, Z., Qian, H., Wang, X., Lin, D., Wang, J., & Xie, L. (2023). Graph neural network-based identification of ditch matching patterns across multi-scale geospatial data. Geocarto International, 38(1), 2294900. 

   <details>
    
   <summary>Synopsis</summary>
   
   [URL](https://www.tandfonline.com/doi/epdf/10.1080/10106049.2023.2294900?needAccess=true)
   
   - Problem: Different scales representing ditches drain rainwater need to be matched  
   - Background:
       - Common GNN types: 
           - graph sample and aggregate (SAG): neighbour sampling / aggregrate functions to extract neighborhood info  
           - topological adaptive graph convolutional (TAGC): skips connections to enhance stronger generlization performance  
   - Approach: supervised GNN 
       - 3 SAGEConv + 1 TAGConv layers
       - Node characterizations: 
           - topological: number of adjacent ditches, connectivity to lakes
           - semantic: hierarchy level; group by width levels 
           - geometric: length of ditch segment 
           - contextual: distribution density of ditch segments
       - Experimented on Netherlands' ditch data
    
   </details>

  
