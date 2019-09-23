FROM tensorflow/tensorflow:latest-py3-jupyter
RUN apt update && apt install tree
RUN mkdir -p /code && mkdir -p /code/static
WORKDIR /code
ADD . /code/
RUN pip install -U pip && pip install -r requirements.txt
RUN jupyter serverextension enable --py jupyterlab