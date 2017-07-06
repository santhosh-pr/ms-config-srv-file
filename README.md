# ms-config-srv-file
Spring cloud config server from local file system

As we are storing the configuration file[data file] local file system, we should enable the profile - **native**
I kept the configuration files to be loaded under the *src/test/resources/config* folder. 
We can specify the path of directory in application.yml file *search-location property*. 

The configuration file [data file] name should be match with application.name in the application.yml file

*we can rename the application.yml by setting the value for spring.config.name as jvm arg*


