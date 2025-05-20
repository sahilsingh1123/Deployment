# Use official python image
FROM python:3.10-slim

# set working directory
WORKDIR /app

# install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# copy application code
COPY . .

# expose service port
EXPOSE 5000

# default command
CMD ["python", "app.py"]


# Steps to build and run docker
# sudo docker build -t flask_app_docker:latest .
# sudo docker run -d -p 5000:5000 --name webservice flask_app_docker:latest
# sudo docker ps -> it will give you list of running images
# sudo docker kill webservice
