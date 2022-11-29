# Base Image
FROM ubuntu:20.04

# Create a workdir
WORKDIR /opt/facebooc

# Copy everything in the path and workdir
COPY . .

# Install update on the base image and install dependencies 
RUN apt-get update && \
    apt-get install -yq build-essential make libsqlite3-dev sqlite3

# Compile the source code
RUN make all

# Expose the image on port 16000
EXPOSE 16000

# launch app
CMD bin/facebooc