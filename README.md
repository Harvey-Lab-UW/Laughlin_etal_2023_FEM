# Laughlin_etal_2023_FEM
Data accompanying the manuscript 'Patterns and drivers of early conifer regeneration following stand-replacing wildfire in Pacific Northwest (USA) temperate maritime forests' by Laughlin, Rangel-Parra, Morris, Donato, Halofsky and Harvey published in Forest Ecology and Management. 
*See the main text of the manuscript for complete descriptions of how data were collected, and greater specifics on values and classifications.*  

[![DOI](https://zenodo.org/badge/750538450.svg)](https://zenodo.org/doi/10.5281/zenodo.10595208)

[![CC BY 4.0][cc-by-shield]][cc-by]

This information is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by]. Any user of these data ("User" hereafter) is required to cite it appropriately in any publication that results from its use. These data may be actively used by others for ongoing research, so coordination may be necessary to prevent duplicate publication. The User is urged to contact the authors of these data for questions about methodology or results.  The User is encouraged to consider collaboration or co-authorship with authors where appropriate. Misinterpretation of data may occur if used out of context of the original study. Substantial efforts are made to ensure accuracy of the data and documentation, however complete accuracy of data sets cannot be guaranteed. All data are made available as is. Data may be updated periodically and it is the responsibility of the User to check for new versions of the data. The authors and the repository where these data were obtained shall not be liable for damages resulting from any use or misinterpretation of the data.

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg


There are two main data files made available for reproducibility purposes:
- plot_level_data.csv
- plot_level_data_by_species.csv


### plot_level_data.csv
This file contains all plot-level variables included in the analyses. The following columns are included:
- **plotID**: unique plot identifier in the format Fire_Plot. 
  - *Fire* is the wildfire where the plot is located (eagl = Eagle Creek, nors = Norse Peak, good = Goodell Creek, mapl = Maple)
  - *Plot* a unique plot number identifier.
- **fire**: the wildfire where the plot is located (eagl = Eagle Creek, nors = Norse Peak, good = Goodell Creek, mapl = Maple)
- **seedling_count**: Raw count of established seedlings >= 10 cm tall within a plot.
- **seedlings_per_ha**: Established seedling density (i.e., seedlings per hectare) >=10 cm tall within a plot
- **seedlings_per_ha_yr**: Establishment rate of seedlings (i.e., seedlings per hectare per year) >=10 cm tall within a plot
- **regen_count**: Raw count of all seedlings within a plot (includes post-fire seedlings of all heights).
- **regen_per_ha**: Seedling density (i.e., seedlings per hectare) within a plot (includes post-fire seedlings of all heights)
- **regen_per_ha_yr**: Regeneration rate of seedlings (i.e., seedlings per hectare per year) within a plot (includes post-fire seedlings of all heights)
- **stand_age**: pre-fire stand age classification of plot (young, mid-seral, or late-seral)
- **forest_zone**: forest zone classification of plot (tshe = western hemlock zone, abam = Pacific silver fir zone) 
- **seedwall_dist_m_sat**: distance in meters to the nearest clump of living mature trees at least 1 ha in area, measured from plot center using 2-3 year post-fire NAIP imagery. Range 22.97 - 1610.11 m.  
- **veg_pc**: average percent cover of herbs and shrubs, measured in the field. Range 0.62 - 57.55% 
- **hli**: plot-level heat load index. An index of incident solar radiation calculated using slope, aspect, and latitude. Values range from 0 (cooler topo-climatic conditions) to 1 (warmer topo-climatic conditions). 
- **twi**: plot-level topographic wetness index. Index of topographic controls on hydrologic processes, including soil moisture. Lower values indicate drier conditions; higher values indicate wetter conditions. Range 4.22 - 8.14. 
- **bryo_pc**: average percent cover of bryophytes (i.e., non-vascular plants), measured in the field. Range 0.10 - 64.09%. 
- **avg_spei_3yr**: Index of growing season drought anomalies over a 180-day window. Values between -1 and 1 indicate relatively ‘normal’ conditions; values < -1 indicate drought; values > 1 indicate a wetter than normal growing season. Range -1.07 - 0.19
- **spp_richness**: number of conifer species present within a plot. Range 1 - 6 species.
- **sdi**: plot-level Shannon diversity index of conifer species. Range 0 - 1.22. 
- **perc_shadeintol**: percentage of total seedlings that are classified as shade intolerant. Range 0 - 100%. 
- **perc_shadetol**: percentage of total seedlings that are classified as shade tolerant.  Range 0 - 100%. 

### plot_level_data_by_species.csv
This file contains regeneration rates (i.e., seedlings per hectare per year, including seedlings of all heights) by species for each plot  The following columns are included:
- **plotID**: unique plot identifier in the format Fire_Plot. 
  - *Fire* is the wildfire where the plot is located (eagl = Eagle Creek, nors = Norse Peak, good = Goodell Creek, mapl = Maple)
  - *Plot* a unique plot number identifier.
- **species**: four letter code indicating the species of each measured conifer seedling.
  - abam = *Abies amabilis*, Pacific silver fir
  - abla = *Abies lasiocarpa*, subalpine fir 
  - abpr = *Abies procera*, noble fir
  - pico = *Pinus contorta*, lodgepole pine
  - pien = *Picea engelmannii*, Engelmann spruce
  - pimo = *Pinus monticola*, western white pine
  - psme = *Pseudotsuga menziesii*, Douglas-fir
  - tshe = *Tsuga heterophylla*, western hemlock 
- **regen_per_ha_yr**: Regeneration rate of seedlings (i.e., seedlings per hectare per year)for a species within a plot (includes post-fire seedlings of all heights).
- **shade_tolerance**: conifer species classification of shade tolerance, binned into two groups: shade intolerant ("intolerant") and shade tolerant ("tolerant"). 


