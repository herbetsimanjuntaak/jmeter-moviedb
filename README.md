# Apache JMeter Load Testing for The Movie Database API

This project provides a load test script for the Movie DB API

## Feature
### Page Person Change endpoint
 - https://api.themoviedb.org/3/person/changes?page=1


### Prerequisites

Prerequisites
Before running the load test, ensure the following:

Apache JMeter is installed on your system.
Java is installed and properly configured.
The required Bearer Token for authorization is available.

### Load Test Configuration
- The load test is configured with the following parameters:
- Thread Number: 2
- Ramp-up Time: 10 seconds
- Duration: 60 seconds
- Endpoint: https://api.themoviedb.org/3/person/changes?page=1
- Authorization
```text
Bearer Token (Bearer eyJhbGciOiJIUzI1NiJ9.eyJhdWQiOiJlNTUwZGFjMjUwMjE4OTQyZjRmOTEzOTFiYjZkY2NjNSIsInN1YiI6IjYwYWY2MDAxYzVjMWVmMDA1OWU2MzVlYiIsInNjb3BlcyI6WyJhcGlfcmVhZCJdLCJ2ZXJzaW9uIjoxfQ.wGzbkGdNmzm7cWjLfyNFVGdpLJKMelfCaoEbUuYs-CA)
```

### Execute the Load Test
#### Run this command to run load test and generate test result:
```txt
jmeter -n -t load_test.jmx -l testreport.jtl
```



### Generate report
#### Run this command to generate test report from test result
```text
jmeter -g testreport.jtl -o filereport
```


### 📝 Reports
![image](https://github.com/user-attachments/assets/10134adf-e6d4-49c3-88b7-c36fbf6a17d9)
