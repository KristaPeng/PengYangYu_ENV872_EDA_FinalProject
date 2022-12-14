# PengYangYu_ENV872_EDA_FinalProject
This is the team repository for the group PengYangYu from Duke University ENV872 course. We are using R to solve real-world related research questions regarding the environment. In this project, we are focusing on the data of ozone concentration in North Carolina, US, from 2016 to 2022. We are eager to study the effect of location, seasons, daily AQI, etc. on ozone concentration using various analysis methods learned from the class.

# Investigators
1. Yanxi Krista Peng: 
Second-Year Master Student of Mechanical Engineering & Materials Science Department
Email Address: yp116@duke.edu
   Role in the Project: Editor of Data Visualization Part (Explanatory Analysis)
2. Kaichun Yang:
   Ph.D Candidate of Mechanical Engineering & Materials Science Department
   Email Address: ky91@duke.edu
   Role in the Project: Editor of Data Wrangling Part
3. Changxin Yu
   Second-Year Master Student of Mechanical Engineering & Materials Science Department
   Email Address: cy182@duke.edu
   Role in the Project: Editor of Data Analysis Part 
   
# Keywords
Environmental Data Analysis, R Studio, Course Project, Duke University, Ozone Concentration, North Carolina, Data Science

# Database Information
Here we studied the ozone concentration trend at North Carolina from 2016 to 2022. The datasets were downloaded directly from EPA Outdoor Air Quality Data section (https://www.epa.gov/outdoor-air-quality-data/download-daily-data).

# Folder structure, file formats, and naming conventions 
The repository contains three folder in total.
1. Code folder
   The rmd files for data wrangling, data visualization, and data analysis can be found in this folder. We also included PDF files for those who have trouble reading rmd files. Each file was directly named after their main subject.
2. Data folder
   In this folder, we included three sub-folder. First, raw datasets that we find online as open resources were contained in the Raw folder. Second, after the process of data wrangling, we collected the data that could used in the project and summarised them into Processed folder. All the files under this two folders are in csv format. We also selected the data that could potentially used in spatial analysis to Spatial. 
3. Output folder
   In this folder, we collected the output image in data visulization and analysis part and each files are either in pdf or png format.
  
# Metadata
In 'Data/Raw' folder:
7 csv files about Ozone in North Carolina from 2016 to 2022, all of them have identical data structureS in different years. The class of data is data.frame.
The column names are: Date, Source, Site ID, POC, Daily Max, UNITS, DAILY_AQI_VALUE, DAILY_OBS_COUNT, PERCENT_COMPLETE, AQS_PARAMETER_CODE, AQS_PARAMETER_DESC, CBSA_CODE, CBSA_NAME, STATE_CODE, STATE, COUNTY_CODE, COUNTY, SITE_LATITUDE, SITE_LONGITUDE.

In 'Data/Processed' folder:
o3_combined.csv is the dataframe that combines the imported raw data. It has the same data structure as the data files in the 'Data/Raw' folder.
o3_cleaned.csv is the dataframe we mainly used for all analysis in this project. It is the simplified version of o3_combined.csv. We have selected 9 columns for this file from o3_combined.csv including Date, Concentration, DailyAQI, SiteName, County, Latitude, Longitude, Month, Year.
o3_fulldate.csv and o3_monthly.csv are for testing purposes and haven't been used.

In 'Data/Spatial' folder:
In this folder, we mainly stored the spatial data for the spatial analysis.
We put 7 files in this folder including cb_2018_us_county_20m.cpg, cb_2018_us_county_20m.dbf, cb_2018_us_county_20m.prj, cb_2018_us_county_20m.shp, cb_2018_us_county_20m.shp.ea.iso.xml, cb_2018_us_county_20m.shp.iso.xml, cb_2018_us_county_20m.shx. 


# Scripts and code
R (with Rstudio)

# Quality assurance/quality control
https://www.epa.gov/outdoor-air-quality-data/download-daily-data

