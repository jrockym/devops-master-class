FROM python:alpine3.10
WORKDIR /app 
COPY requirements.txt /app/requirements.txt
RUN pip install -r requirements.txt
EXPOSE 5000
COPY . /app
# CMD allows command line arguments when container is deployed
# ENTRYPOINT is "static" and doesn't care about args from cmd line
# ENTRYPOINT can overridden with --ENTRYPOINT at command line
CMD python ./launch.py

#
#ENTRYPOINT ["python", "./launch.py"]
