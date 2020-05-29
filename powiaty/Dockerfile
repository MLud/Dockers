FROM rocker/tidyverse
MAINTAINER Michal Ludwicki (Ludwickim@gmail.com)

RUN apt-get -qqy update && apt-get install -qqy \
        openssh-client \
        qpdf
        
## Install packages from CRAN
RUN install2.r --error \ 
    -r 'http://cran.rstudio.com' \
##    googleCloudRunner\
    v8\
    rvest\
    jsonlite\
    lubridate\
	stringr\
## install Github packages
##    && installGithub.r MarkEdmondson1234/googleCloudRunner \

## clean up
    && rm -rf /tmp/downloaded_packages/ /tmp/*.rds
    
    
    

