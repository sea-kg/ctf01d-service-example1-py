FROM python:3.10

WORKDIR /service/app

COPY ./requirements.txt /service/requirements.txt
RUN pip install --no-cache-dir --upgrade -r /service/requirements.txt

COPY ./app /service/app
EXPOSE 4001
CMD ["python3", "-u", "service.py"]