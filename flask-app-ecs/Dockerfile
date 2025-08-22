#Stage-1: current python base image =994 mb ~ 1.04 Gb

FROM python:3.7 AS builder

WORKDIR /app

COPY requirements.txt .

RUN pip install -r requirements.txt

#______________________________________________
# stage-2 : base image :125mb ~ 140 mb

FROM python:3.7-slim

WORKDIR /app

COPY --from=builder /usr/local/lib/python3.7/site-packages/ /usr/local/lib/python3.7/site-packages/

COPY . . 

CMD ["python","run.py"]
