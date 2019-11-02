FROM tensorflow/tensorflow:1.13.1-gpu-py3-jupyter

ADD docker/requirements_os.txt .
RUN apt update -y && apt install -y $(cat requirements_os.txt|grep -v '#')

ADD docker/requirements.txt .
RUN pip install -r requirements.txt
