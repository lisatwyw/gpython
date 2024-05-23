# Python for geospatial analyses

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

  
