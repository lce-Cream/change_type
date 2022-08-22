# Change Type
## Requirements
| Name | Version |
| ------ | ------ |
| Spark | 3.1.3    |
| Docker| 4.7.1   |
| Docker-compose | 1.29.2 |

## Start Spark cluster
Set all necessary variables in ./docker-compose/.env. Then start the cluster.
```bash
cd ./docker-compose
docker-compose up -d
```
Open:
https://localhost:8080 to use Zeppelin;
https://localhost:4040 to see Spark jobs;
https://localhost:7080 to access Spark master node interface.

## Results
### In tables
| 1 worker | 2 workers |
| ------ | ------ |
| <img src="./images/changeType vs changeTypePrevVal on 1 worker 2 cores 2gigs spark cluster.png"> | <img src="./images/changeType vs changeTypePrevVal on 2 workers 2 cores 2gigs spark cluster.png"> |

### In plots
1 worker
<img src="./images/1 worker - 2 cores 2 gigs, no prev value.png">
<img src="./images/1 worker - 2 cores 2 gigs, with prev value.png">
  
2 workers
<img src="./images/2 workers- 2 cores 2 gigs, no prev value.png">
<img src="./images/2 workers- 2 cores 2 gigs, with prev value.png">
