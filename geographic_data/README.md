# 1811_lsoa_to_acute_hospital_travel

This data set includes travel times and distances for all 32,844 Lower Super Output Areas in England (excluding Isles of Scilly) to 185 acute hospitals in England. Tables for inter-hospital travel distances and times are also given.

Data comes from Open Street Map (https://www.openstreetmap.org), and fastest routes were identified using Routino (www.routino.org).

Data files represent raw output from OSM and also and adjusted travel time based on calibration calculated by comparing 200 OSM/Routino route times with Google maps (2am travel times). OSM/Routino tended to under-estimate travel shorter travel times compared with Google.

FILES
=====

correction
----------
Description of the calibration equation for travel times, obtained by comparison of 200 randomly selected routes between OSM/Routino data and Google maps (travel times at 2am Wednesday morning; clear road conditions). 


hospitals.csv
-------------
A list of 185 English acute hospitals with region


inter_hospital_results.csv
--------------------------
Raw Routino output for inter-hospital travel times and distances.


lsoa2011_postcodes.csv
----------------------
Information on lower super output areas and the postcode (closest to population-weighted centroid) used for travel distance/time estimation.


pivoted_distance_km.csv
-----------------------
A pivoted table of LSOA to hospital travel distances (km, fastest road route)


pivoted_inter_hospital_distance_km.csv
---------------------------------------

A pivoted table of inter-hospital travel distances (km, fastest road route)


pivoted_inter_hospital_time_adjusted.csv
----------------------------------------
A pivoted table of inter-hospital travel times (adjusted by calibration against Google maps)


pivoted_inter_hospital_time.csv
-------------------------------
A pivoted table of inter-hospital travel times (not adjusted)


pivoted_time_adjusted.csv
-------------------------
A pivoted table on travel times (fastest road travel time, minutes) from all LSOA to all hospitals (adjusted by calibration against Google maps)


pivoted_time.csv
----------------
A pivoted table on travel times (fastest road travel time, minutes) from all LSOA to all hospitals (not adjusted)


results.csv
-----------
Raw Routino output for travel times and distances from all LSOA to all hospitals.


Note: 2,555 out of 6,075,955 (0.04%) routes did not have a travel time/distances reported by Routino. In that case travel distances were by adjusting straight line distances by the average road distance/straight line distances for all other routes. Travel times were then imputed using an average travel speed for all other routes. 


