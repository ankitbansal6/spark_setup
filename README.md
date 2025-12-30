Create following files and folders structure inside spark-bootcamp folder


### ├── docker-compose.yml

### ├── jupyter/

   └── Dockerfile

### ├── notebooks/

### ├── data/

           └── sample.csv

### ├──event-logs/

### ├──spark-conf/

        └── spark-defaults.conf

Now open windows power shell change directory to spark-bootcamp
Run following commands:  
# Build containers (first time only)
docker compose build

Start Spark Master, Workers, Jupyter
docker compose up -d


Now you should be able to access services on below ports :

Jupyter Lab → http://localhost:8888/
Driver UI → http://localhost:4040
Spark Master UI → http://localhost:8080
Worker 1 UI → http://localhost:8081
Worker 2 UI → http://localhost:8082

# Stop the cluster when done:
docker compose down

# start again when needed 
docker compose up -d

