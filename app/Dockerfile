FROM ubuntu
RUN apt-get update && apt-get install -yq --no-install-recommends \
    python3-pip \
    python3-dev \
    python3-setuptools \
    tesseract-ocr

WORKDIR /app 
COPY ./requirements.txt requirements.txt 
RUN pip3 install --no-cache-dir -r requirements.txt
RUN pip3 install -U scikit-learn
