# data-512-a1

This repository contains the code and resulting data for a brief analysis of English Wikipedia traffic from 2008 - current. It was originally completed for the first assignment of the University of Washington's Human Centered Data Science (DATA 512) course in Autumn 2018. The goal of this assignment was to complete an exercise in data curation, including all major steps in the pipeline, namely data acquisition, processing, and analysis. Another goal was to complete this exercise with reproducibility in mind, ensuring that the documentation for the repository and code are detailed such that somebody else could easily complete the same work.

## Project Organization
This repository contains a jupyter notebook with all necessary code for the project, five raw .json data files resulting from API calls, one .csv containing processed data, and one .png showing the results of the analysis. The repository has the following structure: 

```
data-512-a1/
  |- data_clean/
     |- en-Wikipedia_traffic_200801-201809.csv
  |- data_raw/
     |- pagecount_desktop-site_200801-201809.json
     |- pagecount_mobile-site_200801-201809.json
     |- pageview_desktop_201507-201809.json
     |- pageview_mobile-app_201507-201809.json
     |- pageview_mobile-web_201507-201809.json
  |- results/
     |- wikipedia_traffic_2008-2018.png
  |- src/
     |- hcds-a1-data-curation.ipynb
  |- LICENSE
  |- README.md
```

## Source Data

## API Documentation

## Results
The results of this analysis include a final .csv with processed data and a timeseries plot showing Wikipedia traffic from desktop, mobile, and total views for both the legacy API and the current API. The .csv contains the following fields:

```
 - 'year': str, the year of that data point, in form 'yyyy'
 - 'month': str, the month of that data point, in form 'mm'
 - 'pagecount_all_views': int, total number of views from the pagecount (legacy) API
 - 'pagecount_desktop_views': int, total number of desktop views from the pagecount (legacy) API
 - 'pagecount_mobile_views': int, total number of mobile views from the pagecount (legacy) API
 - 'pageview_total_views': int, total number of views from the pageview (current) API
 - 'pageview_desktop_views': int, total number of desktop views from the pageview (current) API
 - 'pageview_mobile_views': int, total number of mobile views from the pageview (current) API
```
The final timeseries plot, which can be found both in the jupyter notebook in the 'src' directory, or as a .png in the 'results' directory, shows all of the views variables described above plotted over time. 
