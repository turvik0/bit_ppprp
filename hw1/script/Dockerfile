FROM python:3.9-slim
WORKDIR /app
COPY requirements.txt .
RUN pip install requests
COPY script.py .
CMD ["python", "script.py"]
