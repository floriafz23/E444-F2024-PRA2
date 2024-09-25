# Use Python as base image
FROM python:3.10

# Set working directory and copy cwd to container at wd
WORKDIR /app
COPY . /app

# Install everything in requirements.txt
RUN pip3 install -r requirements.txt

# Make port 5000 available to the world outside this container
EXPOSE 5000

# Define flask app
ENV FLASK_APP=hello.py

# Run flask
CMD ["flask", "run", "--host=0.0.0.0"]