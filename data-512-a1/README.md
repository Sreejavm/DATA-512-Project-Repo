# DATA 512 - Assignment 1 - Data Curation

The goal of this project is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through August 30 2020.

## Data Source and License:

The data about Wikipedia page traffic from two different https://www.mediawiki.org/wiki/Wikimedia_REST_APIendpoints have been combined into a single dataset.

The Legacy Pagecounts API (https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts, https://wikimedia.org/api/rest_v1/#/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end) provides access to desktop and mobile traffic data from December 2007 through July 2016.
The Pageviews API (documentation (https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts), endpoint (Links to an external site.)) provides access to desktop, mobile web, and mobile app traffic data from July 2015 through last month.

Licence: Please read the licence and terms of use of Wikimedia Foundation REST API from here.

###Aggregated Final Data:

The final data is present in the file en-wikipedia_traffic_200801-202008.csv.

####Description of fields of the final data: 

year: The year in the YYYY format.
month: The month in MM format.
pagecount_all_views: The view counts from both desktop and mobile collected from Legacy Pagecounts API.
pagecount_desktop_views: The number of views from desktop collected from Legacy Pagecounts API.
pagecount_mobile_views: The number of views from mobile collected from Legacy Pagecounts API.
pageview_all_views: The number of views from desktop, mobile-web and mobile-app users collected from Pageviews API.
pageview_desktop_views: The number of views from desktop users collected from Pageviews API.
pageview_mobile_views: The number of views from mobile-web and mobile-app users collected from Pageviews API.
