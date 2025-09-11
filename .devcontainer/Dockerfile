FROM python:3.11-slim
ARG USERNAME=vscode
WORKDIR /src

COPY requirements.txt .
COPY ./scr ./scr

RUN pip install --no-cache-dir -r requirements.txt


CMD ["uvicorn", "src.main:app", "--host", "0.0.0.0", "--port", "8000"]
