# ms-config-srv-file
Spring cloud config server from local file system

As we are storing the configuration or data file in local file system[doesn’t use Git], we should enable the profile - **native**

I kept the configuration files to be loaded under the *src/test/resources/config* folder. 

Two service confuigurations - ms-employee-svc and ms-dept-svc.

We can specify the path of directory in application.yml file *search-location property*. 

The configuration file [data file] name should be match with application.name of client service mentioned in the application.yml file @ client side - ie ms-employee-svc or ms-dept-svc

*we can rename the application.yml by setting the value for spring.config.name as jvm arg*


we can see the results by invoking the endpoints -- ie the folder name where config files resides.

Dept service

http://localhost:7000/ms-dept-svc/default

http://localhost:7000/ms-dept-svc/dev


Employee service



http://localhost:7000/ms-employee-svc/default

http://localhost:7000/ms-employee-svc/dev




