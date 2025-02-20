```
   mkdir -p ./dags ./logs ./plugins ./config
   echo -e "AIRFLOW_UID=$(id -u)" > .env
   docker compose up -d
   curl -LfO 'https://airflow.apache.org/docs/apache-airflow/2.10.5/airflow.sh'
   chmod +x ./airflow.sh 
   ./airflow.sh 
   ./airflow.sh dags
   ./airflow.sh dags list
   ./airflow.sh dags delete tutorial_taskflow_templates
   ./airflow.sh dags list
   ./airflow.sh dags delete tutorial_taskflow_templates
   ./airflow.sh dags delete -y tutorial_taskflow_templates
```
