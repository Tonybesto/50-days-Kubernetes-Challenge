# Base Image 
FROM python:2.7-alpine

# Using a new working directory
WORKDIR /app

# Copy the requirement files into the working directory
COPY ./requirements.txt /app/requirements.txt

# Install the dependencies and packages
RUN pip install -r requirements.txt

# Copy alll the dependencies into the image
COPY . /app

# Expose on Port 80
EXPOSE 80

# 
CMD ["gunicorn", "app:app", "-b", "0.0.0.0:80"]