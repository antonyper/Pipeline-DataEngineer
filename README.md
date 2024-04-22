# Pipeline Data Engineering con Kafka, Spark, Airflow, Postgres y Docker
Este proyecto se centra en la construcción de un data pipeline usando Kafka, Airflow, Spark y PostgreSQL
## Descripción General:

1. Data Streaming: Los datos se transmiten desde una API a un topic de Kafka
2. Data Processing: Spark job procesa la data desde el topic de Kafka y lo transmite a db PostgreSQL.
3. Scheduling with Airflow: Tanto la tarea de transmisión y los jobs de spark son orquestados por Airflow. Para la demostración, se programará el producer kafka para que se ejecute diariamente. En un escenario real, el producer deberia estar escuchando constantemente a la API.

image/overview.png
