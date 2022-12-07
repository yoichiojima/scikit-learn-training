FROM python:3

COPY requirements.txt /opt
RUN pip install --upgrade pip
RUN pip install -r /opt/requirements.txt

EXPOSE 8888

WORKDIR /home

CMD jupyter lab --ip="0.0.0.0" \
                --port=8888 \
                --LabApp.token="" \
                --allow-root