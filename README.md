

# caplter-birdcommunitydynamics

# A repository for:
Haight, Jeffrey D.; de Albuquerque, Fabio S.; Bateman, Heather L.; Frazier, Amy E.; Larson, Kelli L.. Urbanization and climate drive long-term bird community trends across a desert city ecosystem. _Ecological Applications_

This repository contains code and data used for preparing, analyzing, and visualizing long-term avian point-count data ([Lerman et al. 2023](https://doi.org/10.6073/PASTA/4777D7F0A899F506D6D4F9B5D535BA09)) and relationships between bird occurrence and seasonal environmental conditions at 51 sites across central Arizona, USA ([Haight et al. 2024](https://doi.org/10.6073/PASTA/9D44CD85F881586D6D06E7A7293E833C)). This project is supported by the Central Arizona-Phoenix Long-term Ecological Research (CAP LTER) program

This `README` file includes information on the various R scripts and datasets produced for this analysis. The manuscript includes citation of sources of all used data. This `README` file is organized into three sections corresponding to the three main folders into which the repository is organized
1. [code](#code)  
2. [data](#data)
3. [figures](#figures)

Please direct all questions to Jeffrey Haight jdhaight.eco(at)gmail.com

---
---
<div align="center"> <h3>code</h3> </div>

This folder contains all RMarkdown (.rmd) code files used for synthesizing data and conducting the analyses that produce the manuscript results and `figures` in R. There are a total of seven R scripts, numbered by the order in which they are to be run. Scripts 1_1 and 1_3 are for importing and processing data from their original sources, 2_1 through 2_3 are for conducting the analyses of environmental and bird community trends, and 3_1 is for producing additional maps of environmental data depicted in Appendix S2.


| File  | Description  |
|---|---|
|**./code/1_1_DataCleaning_SpeciesObs_caplter-birdcommunitydynamic.Rmd**   	|For importing and processing raw bird observation datasets sourced from the CAP LTER database|
|**./code/1_2_DataCleaning_SpeciesTraits_caplter-birdcommunitydynamics.Rmd** 	|For importing and processing trait data from the EltonTraits and AVONET databases| 
|**./code/1_3_ModelSetup_caplter-birdcommunitydynamics.Rmd**   			|For organizing datasets in preparation for statistical modeling|
|**./code/2_1_EnvTrends_caplter-birdcommunitydynamics.Rmd**   			|For testing and visualizing spatial-temporal trends in, and relationships among, environmental conditions|
|**./code/2_2_AvianCommunityTrends_caplter-birdcommunitydynamics.Rmd**   	|For testing and visualizing spatial-temporal patterns overall bird community characteristics (abundance and species richness) and functional group abundances|
|**./code/2_3_CommunityGLMM_caplter-birdcommunitydynamics**  			|For fitting generalized linear mixed models examining environmental drivers of overall bird community characteristics (abundance and species richness) and functional group abundances|
|**./code/3_0_SupplementalMaps_caplter-birdcommunitydynamics.R**  		|For creating figures visualizing long-term changes in environmental conditions for Appendix S2|


---
<div align="center"> <h3>data</h3> </div>
This contains all the data files used for conducting the analyses and producing the `figures`.  

| File  | Description  |
|---|---|
|**./data/arizonapalettes.RData**   			|Contains R objects containing manually constructed color palettes for use in figures|
|**./data/bird_observations_countbysurvey.rds** 	|Count data for each bird species, summarized by site, year, season, and survey| 
|**./data/bird_observations_countmeanbyseason.csv**   	|Count data for each bird species sites during each year and season, averaged across surveys (including 0's for non-observed species)|
|**./data/bird_observations_surveycount.rds**   	|Data depicting the number of point-count surveys conducted at each site during each year and season|
|**./data/bird_survey_locations_51sites.shp**   	|ESRI Shapefile depicting the point locations the 51 bird censusing sites selected for analysis|
|**./data/bird_survey_locations_51sites_1000mbuffer.shp**|ESRI Shapefile depicting a 1000-m radius buffer around the 51 bird censusing sites selected for analysis|
|**./data/birdtraits_corebirds2024.csv**  		|Contains synthesized species trait data for all observed bird species|
|**./data/envsummaries_corebirds_combined.csv**		|Long-term environmental data for bird censusing sites (Haight et al. 2024)|
|**./data/modelinputs_CAPbirds2024.RData**		|Contains all cleaned and combined R objects needed to conduct analyses|

---
<div align="center"> <h3>figures</h3> </div>

This folder contains all images utilized in the production of the manuscript figures. This folder includes visualizations produced using the R scripts (see **code** above). These visualizations were then combined within with one another within Inkscape (https://inkscape.org/) to create the figures in the published manuscript. 
