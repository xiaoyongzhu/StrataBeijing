# StrataBeijing
Resources for Strata Beijing

To use this repo:

1.	Download the NYC dataset (usually you just need to download one or two, since if we are analyzing more data then it takes more time and usually doesn’t fit the demo. You can use this one: https://s3.amazonaws.com/nyc-tlc/trip+data/yellow_tripdata_2009-01.csv (it’s around 2.4 GB)
2.	Put the trip data into the wasb folders. In this demo we are using wasb:///NYCData/YellowTrip/rawdata
3.	Install required R libraries in those clusters, using the “Install additional R libraries” command in the script action drop down list:
 
3.1 The libraries need to be installed: "lubridate", "rgeos", "sp", "maptools", "stringr", "magrittr","ggplot2","circlize", "purrr"
4.	Execute this script action to install libgeos in all nodes: https://raw.githubusercontent.com/akzaidi/spark_nyc_taxi/master/Instructor-Resources/Shell-Scripts/libgeos_install.sh 
5.	Execute the R commands as below:
6.	You should be able to see two graphs:
a.	The taxi traffic between different communities for NYC 
b.	The distribution of amount of tips passengers give 
7.	More details on this dataset and what we want to achieve can be found here: https://github.com/akzaidi/spark_nyc_taxi/blob/master/Student-Resources/rmarkdown/3-Visualizing-Taxi-Rides-Spark.Rmd
