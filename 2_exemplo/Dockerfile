FROM python:3.9

WORKDIR /code

COPY ./requirements.txt /code/requirements.txt 

RUN pip install fastapi~=0.79

RUN pip install uvicorn~=0.18

COPY ./app /code/app

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]