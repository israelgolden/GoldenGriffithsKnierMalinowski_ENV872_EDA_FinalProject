# GoldenGriffithsKnierMalinowski_ENV872_EDA_FinalProject
This is the final group project repository for EDA, Spring '22. 

## Summary 

In this project we explore the effects of defaunation, depletion of animals due to hunting, on tropical forest structure and composition. To answer these questions we use a dataset provided by the Poulsen Tropical Ecology lab. This dataset contains tree measurements within forest plots along a defaunation gradient in Ivindo National Park, Gabon. The major takeaways from this data are that there were no apparent relationships between basal area and species richness and the defaunation gradient. These results were unexpected and are most likely a result of faulty data or unit conversion errors. 

## Investigators

Aubrey Knier^1^, Israel Golden^1^, Mishka Malinowski^2^, and Tasha Griffiths^1^
1 - Duke Nicholas School Masters of Environmental Management Candidates
2 - Duke Nicholas School of the Environment - University Program in Ecology PhD Student

## Keywords

Gabon, defaunation, tropical ecology, species composition, gradient, forest structure, basal area, DBH

## Database Information

Data in the repository was collected from the Poulsen Ecology Lab. The data represent forest measurement data from twenty, 50 x 50m forest plots along a defaunation gradient in Ivindo National Park, Gabon. Data collection began in late 2020 and is still ongoing.    


## Folder structure, file formats, and naming conventions 

*Folder structure* -> Data (Processed, Raw, Spatial)
                   -> R_Markdown_Scripts
                   -> GoldenGriffithsKnierMalinowski_ENV872_EDA_FinalProject
                   -> Scratch (misc. things)

*File formats* 

Data folder -> Processed (csv)
            -> Raw (csv, xlsx)
            -> Spatial (two folders Africa and Gabon)
                -> Africa (shapefile and additional necessary files)
                -> Gabon (shapefiles and additional necessary files and csv files with coordinates)

R_Markdown_Scripts -> files in .Rmd format

*Naming Conventions* 
For R markdown scripts -> Last name_analysis type

Final Project -> Last names of all members_class_FinalProject


## Metadata

All data can be found in the Data folder. 

#AUBREY please fix/double check and input tables. 
Raw data is found in the Raw folder within the Data folder and contains a dataset with 21 columns and 45,681 rows. Each row represents a sample or a tree that was measured within the forest plots. Below is a table that described the columns within the dataset:

#BIG TABLE

Processed data is stored in the processed folder within the data folder and was created from wrangling the raw dataset and contains 6,340 rows and 7 columns. A description of the columns is below: 

#SMALL Table 

Spatial data used to create maps of the study site are found in the spatial folder within the data folder. Spatial files are then broken up into more folders - Gabon Country Mask (shapefile of Gabon), National Parks (shapefile of Gabon National Parks), and Plots (shapefile of the forest plots). Additinoally there is a csv file labeled Makokou_Coordinates.csv which gives the latitude and longitude of Makokou the closest large town to Ivindo National Park. 

Column Name | Description | Class of Data | Units
------------|-------------|---------------|-------
City        | Name of city|   nominal     | N/A
Longitude   | coordinates | continuous    | degrees
Latitude    | coordinates | continuous    | degrees


#WE NEED TO DELETE THIS LINE IT WAS JUST FOR GUIDANCE 
<For each data file in the repository, describe the data contained in each column. Include the column name, a description of the information, the class of data, and any units associated with the data. Create a list or table for each data file.> 

## Scripts and code

Final project script and code -> GoldenGriffithsKnierMalinowski_ENV872_EDA_FinalProject.Rmd

All other scripts are in R_Markdown_Scripts folder and are as follows:

Golden_LM.Rmd -> Exploratory analysis for research questions 2 & 3 and linear model synthesis
Griffiths_Wrangling_&_Visualization_DBH.Rmd -> Exploratory analysis for research question 1 
Knier_&_Malinowski_Data_Cleaning_&_Exploration.Rmd -> Raw data wrangling and cleaning
Malinowski_Spatial.Rmd -> Creation of maps for the study site 

## Quality assurance/quality control

Within raw data wrangling and cleaning removed unreasonable samples and those with NAs. Extensive data exploration and application of ecological knowledge of the area. Also met with group members and reviewed each others code. 