## Exploring relationship between household size and car availability
### Introduction
This project aims to explore and visualize the relationship between household size and car availability in England. Car as an important household transportation in the UK, there is an earlier analysis showing that life events are related to the car ownership level (Clark et al., 2014). Some studies also research the relationship between car ownership and family factors, for example, the study from Joachim and Christian (2012) studies the relationship between gender structures and car availability. In the study from point out that households with only 1 adult have a lower possibility of car availability than households with two or more adults. This project will study further explore the relationship between household size and car availability with more detailed data for every factors. Understanding this relationship can help the policymaker for urban planning and transportation policy making.
### Data
DESCRIPTION	SOURCE
household_car.csv	This dataset provides Census 2021 estimates that classify all households in England and Wales by household size.	https://www.nomisweb.co.uk/
Household_size.csv	This dataset provides Census 2021 estimates on the number of cars or vans available to members of households for England and Wales.	https://www.nomisweb.co.uk/
OAC21.csv	This data provides output area classification for 2021	https://data.cdrc.ac.uk/dataset/output-area-classification-2021
Pen_Portraits_EW	This data provides Pen Portraits and Input Variable Listing of output area(2021)	https://data.cdrc.ac.uk/dataset/output-area-classification-2021/resource/pen-portraits-and-input-variable-listing
Oac_england.geojson	This file contains the digital vector boundaries for Output Areas in England and Wales, as at 21 March 2021.	https://geoportal.statistics.gov.uk
Notice: The JSON file is not uploaded to GitHub because the file size is out of limit.

| Variable | Description | mean | std | min | 25% | 50% | 75% | max | Link to source|
|---|---|---|---|---|---|---|---|---|---|
| All usual residents | Number of usual residents in the OA | 309.1149 | 82.97214 | 91 | 264 | 303 | 344 | 4140 | https://www.nomisweb.co.uk |
| Males | Number of Males in the OA | 151.9965 | 45.63066 | 20 | 128 | 148 | 170 | 1994 | https://www.nomisweb.co.uk |
| Females | Number of Females in the OA | 157.1184 | 41.96267 | 12 | 135 | 155 | 176 | 2146 | https://www.nomisweb.co.uk |
| output_area | Output area code | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/dataset/consumer-vulnerability |
| Consumer_Vulnerability | Consumer vulnerability pen portrait | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/dataset/consumer-vulnerability |
| consumer_vulnerability_cluster | Consumer vulnerability cluster | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/dataset/consumer-vulnerability |
| OA_SA | Output area code | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/dataset/output-area-classification-2011 |
| SUB_REGION | Sub region of the UK | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/dataset/output-area-classification-2011 |
| REGION | Region of the UK | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/dataset/output-area-classification-2011 |
| POPULATION | Population of OA | 309.1149 | 82.97214 | 91 | 264 | 303 | 344 | 4140 | https://data.cdrc.ac.uk/dataset/output-area-classification-2011 |
| OAC_super_group_code | Output Area Classification Super Group Code | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/dataset/output-area-classification-2011 |
| OAC_group_code | Output Area Classification Group Code | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/dataset/output-area-classification-2011 |
| OAC_subgroup_code | Output Area Classification Sub-Group Code | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/dataset/output-area-classification-2011 |
| OAC_super_group_name | Output Area Classification Super Group Name | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/output-area-classification-2011/resource/pen-portraits-2011-output-area-classification/resource/pen-portraits-2011-output-area-classification |
| OAC_group_name | Output Area Classification Group Name | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/output-area-classification-2011/resource/pen-portraits-2011-output-area-classification/resource/pen-portraits-2011-output-area-classification |
| OAC_subgroup_name | Output Area Classification Sub-Group Name | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://data.cdrc.ac.uk/output-area-classification-2011/resource/pen-portraits-2011-output-area-classification/resource/pen-portraits-2011-output-area-classification |
| Economically_active_perecentage | % of population economically active | 69.56294 | 9.364096 | 4.9 | 64.2 | 70.3 | 75.7 | 99.1 | https://www.nomisweb.co.uk |
| Economically_active_In_employment_perecentage | % of economically active population in active employment  | 62.00594 | 11.0586 | 0.6 | 56 | 63.4 | 69.4 | 98.2 | https://www.nomisweb.co.uk |
| Economically_active_Unemployed_perecentage | % of economically active unemployment | 4.422425 | 3.085969 | 0 | 2.2 | 3.6 | 5.9 | 46.9 | https://www.nomisweb.co.uk |
| Economically_active_Full-time_student_perecentage | % of economically active population that are full time students | 3.134178 | 2.715611 | 0 | 1.7 | 2.7 | 3.8 | 55.5 | https://www.nomisweb.co.uk |
| Economically_Inactive_perecentage | % of population that are economically inactive | 30.43704 | 9.364099 | 0.9 | 24.3 | 29.7 | 35.8 | 95.1 | https://www.nomisweb.co.uk |
| Economically_inactive_Retired_perecentage | % of population that are economically inactive and retired | 14.54672 | 8.154455 | 0 | 8.7 | 13.4 | 19 | 93.8 | https://www.nomisweb.co.uk |
| Economically_inactive_Student_including_full-time_students_perecentage | % of population that are economically inactive and students | 5.119019 | 5.590758 | 0 | 2.7 | 4 | 5.8 | 88.4 | https://www.nomisweb.co.uk |
| Economically_inactive_Looking_after_home_or_family_perecentage | % of population that are economically inactive and are looking after family/home | 4.318384 | 2.658258 | 0 | 2.5 | 3.8 | 5.5 | 39.4 | https://www.nomisweb.co.uk |
| Economically_inactive_Long-term_sick_or_disabled_perecentage | % of population that are economically inactive and are sick or disabled  | 4.340841 | 3.828691 | 0 | 1.6 | 3.2 | 6 | 46.1 | https://www.nomisweb.co.uk |
| Economically_inactive_Other_perecentage | % of population that are economically inactive that are not retired, students, looking after the home, sick or disabled | 2.111315 | 2.14308 | 0 | 0.9 | 1.7 | 2.8 | 75.2 | https://www.nomisweb.co.uk |
| 2011_output_area | Output area code | NaN | NaN | NaN | NaN | NaN | NaN | NaN | https://www.nomisweb.co.uk |
