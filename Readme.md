For running the airflow webserver and scheduler along with Redis and postgresql

Follow the below setup to make it up and running:

1) Prerequisites: docker installed, docker compose installed
2) Clone the repo
3) Run command: echo -e "AIRFLOW_UID=$(id -u)\nAIRFLOW_GID=0" > .env (to set the environment variable in .env. It will created the .env by itself)
4) Run command: docker-compose -f ./airflow-docker-compose.yml up airflow-init
5) Run command: docker-compose -f ./airflow-docker-compose.yml up
6) Check at http://localhost:8082