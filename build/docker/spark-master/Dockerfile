ARG spark_version
FROM spark-base:${spark_version}

# -- Runtime

# ARG spark_master_web_ui_port=8080
# EXPOSE ${spark_master_web_ui_port} ${SPARK_MASTER_PORT} ${SPARK_UI_PORT}
EXPOSE 8080 7077
CMD bin/spark-class org.apache.spark.deploy.master.Master >> logs/spark-master.out