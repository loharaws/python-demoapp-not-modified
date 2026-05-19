FROM python:3.11-slim

WORKDIR /app

ARG srcDir=src

COPY ${srcDir}/requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

COPY ${srcDir}/ .

EXPOSE 5000

CMD ["python", "run.py"]
