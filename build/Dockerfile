FROM python:3.11-slim
WORKDIR /app
ARG srcDir=src
COPY $srcDir/requirements.txt ./app
RUN pip install --no-cache-dir -r requirements.txt
COPY $srcDir/app ./app
COPY $srcDir/run.py .

EXPOSE 5000

CMD ["python", "app.py"]
