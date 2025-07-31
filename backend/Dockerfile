FROM python:3.13.5-alpine

WORKDIR /app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 5000
CMD ["flask", "--app", "src.app", "run", "--debug", "--host=0.0.0.0"]
# flask --app src.app run --host=0.0.0.0 --port=5001 --debug
