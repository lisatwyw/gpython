# References

## Reviews

Vijayakumar, S., Saravanakumar, R., Arulanandam, M., & Ilakkiya, S. (2024). Google Earth Engine: empowering developing countries with large-scale geospatial data analysis—a comprehensive review. Arabian Journal of Geosciences, 17(4), 1-20.
https://doi.org/10.1007/s12517-024-11948-x

<details>
  
  <summary>Notes</summary>

  Google Earth Engine (GEE) was compared to ArcGIS, QGIS
  - GEE
    - Steep learning curve
    - Seemless integration with other Google products (Google- Maps, Earth)
    - Easy code sharing
  - ArcGIS/QGIS:
    - Easy to use GUI
    - Data is stored and processed locally on users' computerss
     
  
  
</details>

## Disaster management
 
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
