# Use alpine linux as a base image
FROM alpine:3.9

# Set the working directory to /app
WORKDIR /app

#Install uwsgi package
RUN apk add --no-cache uwsgi-python3 && \
    pip3 install --upgrade pip

# Copy the current directory contents into the container at /app
COPY ./app /app

# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt

# Define environment variable
ENV NAME World