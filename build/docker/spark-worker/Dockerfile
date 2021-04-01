ARG spark_version
FROM spark-base:${spark_version}

# -- Runtime

# ARG spark_worker_web_ui_port=8081
# EXPOSE ${spark_worker_web_ui_port}
EXPOSE 8081
CMD bin/spark-class org.apache.spark.deploy.worker.Worker spark://${SPARK_MASTER_HOST}:${SPARK_MASTER_PORT} >> logs/spark-worker.out