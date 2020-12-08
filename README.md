### Ocean's 4 Capstone CSE583 Project
# Phoenix 
[![Build Status](https://travis-ci.org/emilysellinger/phoenix.svg?branch=main)](https://travis-ci.org/emilysellinger/phoenix) [![Coverage Status](https://coveralls.io/repos/github/emilysellinger/CSE583-Project/badge.svg)](https://coveralls.io/github/emilysellinger/CSE583-Project)

Phoenix offers an researchers an intial analysis of the impact of the 2020 Oregon wildfires on bird observations in the state. We use detailed citizen scientist data from eBird and air quality data from the Oregon Department of Environmental Quality to compare sightings with PM2.5 levels. 

Science communication is a growing priority among researchers. To encourage community engagement, Phoenix also includes a visualization tool to be accessed by recreational birders. If made widely available as an interactive map on a website, birders will be able to use this information to gain a better understanding of how to adjust their practices and get the most out of their experience.

### Organization
The project has the following structure:
<pre>phoenix/
  |- README.md
  |- phoenix/
     |- data/
        |-Daily_Avg_PM2.5_Location.csv
        |- ORAQ_StationCounties.csv
        |- OR_DailyAQ_byCounty.csv
        |- Oregon_Resident_Species.md
        |- Oregon_counties_map.geojson
        |- PM2.5_metadata.txt
        |- shortened_bird_data.csv
     |- demos/
        |- Demo_Researcher Use Case.ipynb
     |- code/
        |- air_quality_knn.py
        |- app.py
        |- data_cleaning.py
        |- travis_test.py
     |- tests/
        |- ... 
  |- docs/
     |- ComponentSpecification.md
     |- FunctionalSpecification.md
     |- TechnologyReview.pdf
     |- Presentation.pdf
  |- .travis.yml
  |- Licence.md
  |- environment.yml
</pre>
### How to Use Phoenix
Researchers should look to our demo jupyter notebook, where you can find a more detailed description of our analysis, as well as accompanying visualizations.Phoenix uses Altair for statistical visualizations, the code for which can be easily adapted for future research.
For recreational birders, we provide a dash app where you can explore resident species observations and air quaility index (AQI) at several geographic and taxonomic levels.
To explore the data on your own, clone the repository onto your device and create an environment using the following code:
<pre>conda env create -f environment.yml</pre>
