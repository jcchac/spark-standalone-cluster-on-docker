FROM spark-base

# Runtime

ARG spark_master_web_ui_port=8080

EXPOSE ${spark_master_web_ui_port} ${SPARK_MASTER_PORT}
CMD bin/spark-class org.apache.spark.deploy.master.Master >> logs/spark-master.out