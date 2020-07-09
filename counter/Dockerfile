FROM balenalib/raspberrypi3-debian-python:3.7-buster-build

WORKDIR /usr/app/src
RUN apt-get update && apt-get install -y ttf-dejavu
RUN pip install pillow RPi.GPIO influxdb adafruit-circuitpython-rgb-display spidev
COPY *.py ./

CMD ["python","counter.py"]
