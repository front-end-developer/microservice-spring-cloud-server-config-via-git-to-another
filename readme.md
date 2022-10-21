### Java Spring boot microservices 
#### for learning only
##### Author: Mark W

This example app communicates with the another git repo, just to get configuration settings stored in another git repo:
namely : https://github.com/front-end-developer/microservice-spring-cloud-server-config-via-git

In this exercise I search to pull all files under the folders starting with the name 'station' with the yaml setting:

    search-paths: station*


In example setting also created a repo called 'perf', also searches anything under the directory named 'station/*' from an additional repo called:
https://github.com/front-end-developer/microservice-spring-cloud-server-config-via-git-to-another-2

to run do: 

    ./mvnw spring-boot:run

then in postman test:
- http://localhost:8888/s1rates/default/main
- http://localhost:8888/s1rates/dev/main
- http://localhost:8888/s2rates/default/main
- http://localhost:8888/s2rates/dev/main