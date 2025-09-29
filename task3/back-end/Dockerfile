FROM ubuntu:latest
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update \
 && apt-get upgrade -y \
 && apt-get install -y python3 python3-pip curl ca-certificates \
 && apt-get clean \
 && rm -rf /var/lib/apt/lists/*

# If EXTERNALLY-MANAGED issue appears, uncomment:
# RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

RUN pip3 install --no-cache-dir flask flask-cors

WORKDIR /app
COPY ./api.py /app/api.py

EXPOSE 5252
CMD ["python3", "api.py"]
