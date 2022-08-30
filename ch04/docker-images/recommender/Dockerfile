FROM  tensorflow/tensorflow:1.12.0-devel-py3
RUN pip3 install --upgrade pip
RUN pip3 install pandas --upgrade
RUN pip3 install keras --upgrade
RUN pip3 install minio --upgrade
RUN mkdir -p /opt/kubeflow
COPY RecommenderKubeflow.py /opt/kubeflow/
ENTRYPOINT ["python3", "/opt/kubeflow/RecommenderKubeflow.py"]
