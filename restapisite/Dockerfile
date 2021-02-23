# The first instruction is what image we want to base our container on
# We Use an official Python runtime as a parent image
FROM python:3.7

# The enviroment variable ensures that the python output is set straight
# to the terminal with out buffering it first
ENV PYTHONUNBUFFERED 1

# create root directory for our project in the container and Set the working directory
RUN mkdir /app
WORKDIR /app
COPY requirements.txt /app/
# Install dependencies
RUN pip install -r requirements.txt
COPY . /app
