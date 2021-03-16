FROM python:3.7

RUN pip install fastapi uvicorn nest-asyncio pydantic pyngrok python-multipart numpy pandas torch tensorflow transformers

EXPOSE 8000

RUN mkdir /app

WORKDIR /app

COPY . /app

CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]